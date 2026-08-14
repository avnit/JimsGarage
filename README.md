[Discord](https://discord.gg/qW5vEBekz5) <br>
[Twitter](https://twitter.com/jimsgarage_) <br>
[Reddit](https://www.reddit.com/user/Jims-Garage)

![alt text](https://github.com/JamesTurland/JimsGarage/blob/main/Logo/Jim'sGarage-1(2).png?raw=true)

# Jim's Garage
Here's a collection of Docker Compose and config files for use in my videos. Simply tweak to your environment and deploy!

## Star History

<a href="https://star-history.com/#JamesTurland/JimsGarage&Date">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=JamesTurland/JimsGarage&type=Date&theme=dark" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=JamesTurland/JimsGarage&type=Date" />
   <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=JamesTurland/JimsGarage&type=Date" />
 </picture>
</a>

<!-- ARCH-DIAGRAM:START -->

## Architecture

> Auto-generated architecture diagram. See [`docs/context-map.md`](docs/context-map.md) for the full context map (core application, containers/cloud, and database connections).

```mermaid
flowchart TD
  User([User / Client])
  App["JimsGarage"]
  DB0[("PostgreSQL / AlloyDB")]
  DB1[("MySQL / MariaDB")]
  DB2[("MongoDB")]
  DB3[("Redis")]
  SVC0["Cloudflare Workers"]
  Img["Container image<br/>(Docker/Compose)"]
  Deploy["GKE / Kubernetes"]
  User --> App
  App --> DB0
  App --> DB1
  App --> DB2
  App --> DB3
  App --> SVC0
  App -.deploy.-> Img
  Img -.deploy.-> Deploy
```

<!-- ARCH-DIAGRAM:END -->
