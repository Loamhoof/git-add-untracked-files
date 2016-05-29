#!/usr/bin/env bash

files=$( git ls-files --others --exclude-standard )

for file in $files; do
    read -p "Add $file [y,N,r]?"
    if [[ $REPLY =~ ^[yY]$ ]]; then
        git add $file
    elif [[ $REPLY =~ ^[rR]$ ]]; then
        rm $file
    fi
done
