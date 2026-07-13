---
title: "Secure Image Uploads in Next.js With Signed Uploads and Cloudinary"
url: "https://cloudinary.com/blog/nextjs-secure-image-uploads"
date: "2026-06-11"
author: "melindapham"
feed_url: "https://cloudinary.com/blog/feed/"
---
Stop exposing your API Secret. Here’s how to do image uploads the right way. Live demo: nextjs-secure-image-uploads.vercel.app Full source: github.com/musebe/nextjs-secure-image-uploads The Problem Every Developer Runs Into Production apps need to prove that an upload request came from your app, not a third party. The way to do that with Cloudinary is a server-generated signature . Your server...
