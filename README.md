# Cloudflare DNS & Security Implementation 🛡️

## Project Overview
This project focuses on improving the security, performance, and reliability of a live website (**apexflora.co.uk**) by integrating it with Cloudflare’s global edge network. The implementation demonstrates practical understanding of DNS management, traffic proxying, and web security fundamentals.

---

## Objectives
- Protect origin server from direct exposure  
- Enable secure HTTPS traffic  
- Improve latency using CDN distribution  
- Gain hands-on experience with real-world web infrastructure  

---

## Implementation Details

### 1. DNS & Nameserver Migration
- Migrated authoritative DNS from IONOS to Cloudflare  
- Updated domain to use Cloudflare nameservers:
  - `nola.ns.cloudflare.com`
  - `woz.ns.cloudflare.com`
- Ensured zero downtime during propagation  

---

### 2. CDN & Proxy Configuration
- Enabled Cloudflare proxy (Orange Cloud) to:
  - Hide origin IP  
  - Filter malicious traffic  
- Leveraged CDN caching to improve content delivery speed  

---

### 3. SSL/TLS & Secure Traffic
- Enabled Universal SSL for HTTPS encryption  
- Configured DNS records (A, CNAME) for correct routing  
- Ensured secure communication between client and edge  

## Verification & Testing

### HTTP Header Validation
Used `curl` to verify Cloudflare proxy status:
<img width="1918" height="642" alt="cloudflare implementation" src="https://github.com/user-attachments/assets/9473e882-1d02-4085-b218-b4aef079e281" />

```bash
curl -I https://apexflora.co.uk


