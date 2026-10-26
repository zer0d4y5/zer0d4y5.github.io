# zer0d4y5.github.io

Security research by Elias Hasas ([@zer0d4y5](https://github.com/zer0d4y5)).

The write-ups are published on the [Brickell Technologies blog](https://brickell-tech.com/blog). This site
is a link page, and the old post URLs redirect to the matching articles there.

- [CVE-2026-110720: A ServiceAccount Name Was Enough to Become Consul Admin](https://brickell-tech.com/blog/consul-k8s-cross-namespace-acl-bypass-cve-2026-110720)
- [FZ-2026-008: Firezone Gateways Trusted the Proxy IPs Clients Sent Them](https://brickell-tech.com/blog/firezone-gateway-proxy-ip-bypass-fz-2026-008)
- [CVE-2026-114615: Off by One Newline, or How Authlib's JWT Algorithm Confusion Came Back](https://brickell-tech.com/blog/authlib-algorithm-confusion-incomplete-fix-cve-2026-114615)
- [CVE-2026-105937: Reading Another Tenant's Messages Through an Apache Pulsar Shadow Topic](https://brickell-tech.com/blog/apache-pulsar-shadow-topic-cross-tenant-cve-2026-105937)
- [CVE-2026-112947: Reading Past Vite's server.fs Boundary Through a WebAssembly Error](https://brickell-tech.com/blog/vite-wasm-instance-fs-bypass-cve-2026-112947)
- [CVE-2026-110779 and CVE-2026-110780: Two Memory-Safety Bugs in Netatalk's Spotlight RPC](https://brickell-tech.com/blog/netatalk-spotlight-cve-2026-110779-cve-2026-110780)
- [CVE-2026-96615: Cross-Namespace Agent Impersonation in NGINX Gateway Fabric](https://brickell-tech.com/blog/nginx-gateway-fabric-agent-impersonation-cve-2026-96615)
- [CVE-2026-85184: When your router and your middleware read different URLs](https://brickell-tech.com/blog/fastify-middie-auth-bypass-cve-2026-85184)
- [CVE-2026-41992: The gzip patch that fixed the crash and left the bug](https://brickell-tech.com/blog/gzip-incomplete-patch-cve-2026-41992)

| Old URL | Redirects to |
|---|---|
| `/posts/middie-cve-2026-85184/` | the @fastify/middie article |
| `/posts/gzip-cve-2026-41992/` | the gzip article |
| `/posts/gzip-lzh-walkthrough/` | the gzip article |

Static HTML, no build step. `.nojekyll` is present so GitHub Pages serves the files as-is.
