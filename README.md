# ShelfPod Legal

Static legal pages for ShelfPod.

- Privacy Policy: `/privacy/`
- Terms of Use: `/terms/`

## Cloudflare Pages

Use these settings when connecting this repository in Cloudflare Pages:

- Framework preset: `None`
- Build command: leave empty
- Build output directory: `public`

After deployment, configure the public URLs in App Store Connect and in the ShelfPod app:

- Privacy Policy URL: `https://<your-domain>/privacy/`
- Terms of Use URL: `https://<your-domain>/terms/`

For an Aliyun-managed domain, add the DNS record requested by Cloudflare when you attach the custom domain. A common setup is:

- Type: `CNAME`
- Name: `legal`
- Value: the Cloudflare Pages target shown in the custom domain setup

This gives:

- `https://legal.<your-domain>/privacy/`
- `https://legal.<your-domain>/terms/`
