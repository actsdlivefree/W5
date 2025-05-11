START_DATE="2025-02-01"
DAYS=10
FILE="README.md"

for ((i=0; i<$DAYS; i++)); do
  COMMIT_DATE=$(date -d "$START_DATE +$i days" "+%Y-%m-%dT12:00:00")
  echo "Commit on $(date -d "$START_DATE +$i days" "+%Y-%m-%d")" >> $FILE
  git add $FILE
  GIT_AUTHOR_DATE="$COMMIT_DATE" GIT_COMMITTER_DATE="$COMMIT_DATE" git commit -m "Auto commit on $(date -d "$START_DATE +$i days" "+%Y-%m-%d")"
done

echo "✅ Done generating fake commits."
Commit on 2025-03-01
Commit on 2025-03-02
Commit on 2025-03-03
Commit on 2025-03-04
Commit on 2025-03-05
Commit on 2025-03-06
Commit on 2025-03-07
Commit on 2025-03-08
Commit on 2025-03-09
Commit on 2025-03-10
Commit on 2025-03-11
Commit on 2025-03-12
Commit on 2025-03-13
Commit on 2025-03-14
Commit on 2025-03-15
Commit on 2025-03-16
Commit on 2025-03-17
Commit on 2025-03-18
Commit on 2025-03-19
Commit on 2025-03-20
Commit on 2025-03-21
Commit on 2025-03-22
Commit on 2025-03-23
Commit on 2025-03-24
Commit on 2025-03-25
Commit on 2025-03-26
Commit on 2025-03-27
Commit on 2025-03-28
Commit on 2025-03-29
Commit on 2025-03-30
Commit on 2025-03-31
Commit on 2025-04-01
Commit on 2025-04-02
Commit on 2025-04-03
Commit on 2025-04-04
Commit on 2025-04-05
Commit on 2025-04-06
Commit on 2025-04-07
Commit on 2025-04-08
Commit on 2025-04-09
Commit on 2025-04-10
Commit on 2025-04-11
Commit on 2025-04-12
Commit on 2025-04-13
Commit on 2025-04-14
Commit on 2025-04-15
Commit on 2025-04-16
Commit on 2025-04-17
Commit on 2025-04-18
Commit on 2025-04-19
Commit on 2025-04-20
Commit on 2025-04-21
Commit on 2025-04-22
Commit on 2025-04-23
Commit on 2025-04-24
Commit on 2025-04-25
Commit on 2025-04-26
Commit on 2025-04-27
Commit on 2025-04-28
Commit on 2025-04-29
Commit on 2025-04-30
Commit on 2025-05-01
Commit on 2025-05-02
Commit on 2025-05-03
Commit on 2025-05-04
Commit on 2025-05-05
Commit on 2025-05-06
Commit on 2025-05-07
Commit on 2025-05-08
Commit on 2025-05-09
Commit on 2025-05-10
Commit on 2025-05-11
