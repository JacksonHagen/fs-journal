# SQL

```sql
SELECT
 a.*,
 g.*,
 m.id AS memberId
FROM members m --many to many object
JOIN groups g ON m.groupId = g.id --many to one object
JOIN accounts a ON g.creatorId = a.id --object #2 creatorId and accountId
WHERE m.profileId = @id -- where the member id = the profile id
```

```csharp
internal List<GroupMemberViewModel> GetByProfileId(string id) {
 string sql = @"
 SELECT
  a.*,
  g.*,
  m.id AS memberId
 FROM members m
 JOIN groups g ON m.groupId = g.id
 JOIN accounts a ON g.creatorId = a.id
 WHERE m.profileId =@id
 "
return _db.Query<Account, GroupMemberViewModel, GroupMemberViewModel>(sql, (a, g) => {
 g.Creator = a;
 return g;
}, new { id }).ToList();
}
```
