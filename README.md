# ShelfPod Legal

Static legal pages for ShelfPod.

- Privacy Policy: `/privacy/`
- Terms of Use: `/terms/`

## Cloudflare Pages

Use these settings when connecting this repository in Cloudflare Pages:

- Framework preset: `None`
- Build command: leave empty
- Build output directory: `public`

Or deploy with Wrangler after logging in:

```sh
npx wrangler login
npx wrangler pages project create shelfpod --production-branch main
npx wrangler pages deploy public --project-name shelfpod --branch main
```

After deployment, configure the public URLs in App Store Connect and in the ShelfPod app:

- Privacy Policy URL: `https://<your-domain>/privacy/`
- Terms of Use URL: `https://<your-domain>/terms/`

For an Aliyun-managed domain, add the DNS record requested by Cloudflare when you attach the custom domain. A common setup is:

- Type: `CNAME`
- Name: `shelfpod`
- Value: the Cloudflare Pages target shown in the custom domain setup

This gives:

- `https://shelfpod.<your-domain>/privacy/`
- `https://shelfpod.<your-domain>/terms/`
