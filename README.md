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
