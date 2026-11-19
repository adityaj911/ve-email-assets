# ve-email-assets

Public image assets for Venkateshwara Enterprises email campaigns. This repository
exists so that marketing emails can reference images by URL instead of embedding them
as attachments — an email then weighs about 12 KB instead of 440 KB.

## Serving

Images are served through the jsDelivr CDN, which has an edge node in Mumbai:

```
https://cdn.jsdelivr.net/gh/adityaj911/ve-email-assets@<tag>/<path>
```

**Always reference a tag, never a branch.** A tag is immutable, so an email sent today
keeps rendering correctly years later even if the repository is reorganised. A branch
reference would break every email already in people's inboxes the moment a file moves.

## Layout

```
brand/                   logos reused across every campaign
ve-insights/<YYYY-MM>/   creatives for one issue of the VE Insights newsletter
```

A new issue gets a new dated folder and a new tag. Earlier tags are never changed.

## Note

This repository is public, which is what allows mail clients to load the images.
Nothing confidential belongs here.
