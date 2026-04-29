# Vercel MCP

**Provider:** claude.ai  
**Status:** △ needs authentication  
**Type:** Deployment / Hosting / Edge Functions

## Overview

Vercel MCP connects Claude to your Vercel account, enabling project deployment, domain management, environment variable configuration, and deployment log inspection. Requires authentication before first use.

## Authentication

```
Step 1: Run authenticate tool → prompts for Vercel OAuth or token
Step 2: Complete sign-in in browser (or paste a Vercel access token)
Step 3: Run complete_authentication tool → confirms connection
```

Get a token at: https://vercel.com/account/tokens

## Available Tools (post-auth)

| Tool | Description |
|------|-------------|
| `authenticate` | Initiate Vercel authentication |
| `complete_authentication` | Finalize the authentication handshake |

Once authenticated, Claude gains access to Vercel operations including:
- Listing and inspecting projects and deployments
- Triggering new deployments (from Git or CLI)
- Viewing build and runtime logs
- Managing environment variables per environment (production/preview/development)
- Managing domains and DNS records
- Inspecting Edge Function and Serverless Function usage

## Usage Examples

```
Show me the last 5 deployments for my-app and their status

What are the environment variables set for production on my-nextjs-project?

Add a new env var STRIPE_SECRET_KEY to production on checkout-service

Show me the build logs for the failed deployment from 2 hours ago

List all my Vercel projects and their frameworks
```

## Notes

- Requires a Vercel account (Hobby, Pro, or Enterprise)
- Team projects require a token scoped to the correct team
- Triggering deployments via MCP is equivalent to running `vercel --prod`
- Environment variable values are write-only in some scopes for security
