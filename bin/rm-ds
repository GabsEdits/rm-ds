#!/bin/bash

# Set the directory to search (default is the current directory)
DIR="${1:-.}"

# Count the number of deleted files

count=0

# Find and delete .DS_Store files, and log each deletion
while IFS= read -r -d '' file; do
  if rm "$file"; then
    echo "Deleted: $file"
    ((count++))
  else
    echo "Failed to delete: $file"
  fi
done < <(find "$DIR" -name '.DS_Store' -type f -print0)

# Print the total number of deleted files
echo "Total .DS_Store files deleted: $count"
