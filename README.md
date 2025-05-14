# *Upgrading my homelab 2025*

For now, my homelab is only a NextCloud server.
I want to upgrade it, and train on my Kubernetes skills.

# *Homelab Tech Slack: (gets update)*
1. **Laptop**: 
   - Asus rog GL552VL: 
      - i7-6700HQ, GTX 965M, 32G RAM (Used to be a gaming laptop)
   - Runs: Ubuntu Server 22.04.5 LTS
3. **NextCloud server**:
   - ~~hosted on ports 80/443 with DuckDNS (for now)~~ Hosted with CloudFlare
   - maintaind and updated
4. **k3s**:
   - manage pods, clusters and nodes
   - nginx ingress: because i'm using ports 443/80 for NextCloud I switched from Traefik ingress to ngnix on another ports.
5. **DevPod**:
   - working on DevPos containers to isolate working enviroments
6. **Flux**:
   - CD of Kubenetes
7. **Host**: **CloudFlare**
   - morielclouds.com
   - Used CloudFlared to host the pods to the internet
8. **Managed secret with SOPS**
   - Cloudflare tunnel
   - linkding enviorment for SU

# *Apps*
1. **Linkding**: Bookmark manager
2. **Prometheus**: Monitor app -> hosted localy with ngnix-ingress
3. **Renovate**: Auto version control: detects upgraded version, updates the YAMLs and make a pull request.
4. **AudioBookShelf**: added for fun, it's tunred off for now
5. **Pi-Hole**: Self hosted DNS server -> hosted localy with ngnix-ingress
6. **Homepage**: To see all the homelabs pods and info -> hosted localy with ngnix-ingress
