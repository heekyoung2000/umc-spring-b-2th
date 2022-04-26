/*게시물 조회*/
SELECT f.nickName, useridx, ImgUrl, content, postidx,
        IF(postCount is null, 0, postCount) as postCount

FROM Feed as f
    left join (SELECT nickName, COUNT(postidx) as postCount
               FROM Feed
               group by nickName) u on u.nickName = f.nickName
WHERE f.useridx = 1;

/*게시물 올린 시간 조회*/
SELECT f.nickName, useridx, postidx, f.updatedAt,
        IF(postCount is null, 0, postCount) as postCount
FROM Feed as f
    left join(SELECT updatedAt, COUNT(postidx) as postCount
              FROM Feed
            group by updatedAt) u2 on u2.updatedAt = f.updatedAt
WHERE f.useridx = 2;

/*게시물 좋아요 개수 조회*/
SELECT f.nickName, useridx, postidx, likeidx,
        IF(postCount is null, 0, postCount) as postCount,
        IF(likeCount is null, 0, likeCount) as likeCount
FROM Feed as f
    left join(SELECT COUNT(likeidx) as likeCount, COUNT(postidx) as postCount
            FROM Feed
            group by likeidx) l on l.likeCount = likeCount
