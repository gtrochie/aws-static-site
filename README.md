# Cloud Static Site on AWS S3

A personal website hosted on Amazon S3 using static website hosting.
Built as my solo project for the WeThinkCode_ Cloud Computing elective.

## What it does

My website's files (HTML and CSS) live in an Amazon S3 bucket. S3's static
website hosting feature serves those files directly as a public web page, so
there's no server for me to manage — AWS serves the files for me.

## Tech used

- **HTML / CSS** — the site itself, hand-written
- **Amazon S3** — stores the files and serves them as a static website
- **S3 bucket policy** — grants public read-only access to the files
- **Git / GitHub** — version control and project history

## How it's set up

1. Created an S3 bucket in the `af-south-1` (Cape Town) region.
2. Uploaded `index.html` and `style.css` to the bucket.
3. Enabled **Static website hosting** in the bucket properties, with
   `index.html` as the index document.
4. Turned off "Block all public access" so the site can be viewed publicly.
5. Added a **bucket policy** allowing `s3:GetObject` (read only) to everyone —
   anyone can view the files, nobody can change or delete them.

## Demo

📹 Video walkthrough: https://youtu.be/QDpjgf7IcIk




















**veriification code:** `WTC-SZW8PGT2`