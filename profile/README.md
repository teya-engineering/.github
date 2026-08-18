<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/teya-engineering/.github/main/profile/assets/banner-dark.png">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/teya-engineering/.github/main/profile/assets/banner-light.png">
  <img alt="Teya Engineering - open source from the team building payments for local business" src="https://raw.githubusercontent.com/teya-engineering/.github/main/profile/assets/banner-light.png">
</picture>

<p align="center">
  <a href="https://www.teya.com"><img alt="Website" src="https://img.shields.io/badge/Website-teya.com-DDE048?style=for-the-badge&labelColor=151515"></a>
  <a href="https://www.teya.com/blog"><img alt="Blog" src="https://img.shields.io/badge/Blog-read-DDE048?style=for-the-badge&labelColor=151515"></a>
  <a href="https://jobs.ashbyhq.com/teya"><img alt="Careers" src="https://img.shields.io/badge/Careers-we're%20hiring-DDE048?style=for-the-badge&labelColor=151515"></a>
  <a href="https://www.linkedin.com/company/teya-global"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-follow-DDE048?style=for-the-badge&labelColor=151515"></a>
</p>

---

## We keep the money side of local business moving

Teya builds payments, business accounts, and funding for small businesses across Europe. A card machine on the counter of a bakery. Instant settlement for a barber shop on a Friday night. An account that handles the boring parts of the books so the owner can go home.

More than 75,000 businesses run on what we build. Real money, in real time, with no good day to be down. That sets the bar for the software behind it.

This is where we share the parts of that work we think are useful to everyone else.

## How we build

We run a lot of services, and we would rather they were boring. The interesting part of a payments platform should be the payments, not the plumbing.

- **The JVM does the heavy lifting.** Java and Kotlin on Spring Boot for most services, on the current LTS or better.
- **Events over calls.** Kafka carries most of what moves between services, with schemas that are versioned and checked before anything ships.
- **Postgres until it hurts.** Then we partition it. We are slow to add a new datastore and quick to lean on the one we know.
- **If we cannot see it, it is not done.** Metrics, logs, and traces are part of the change, not a follow-up ticket.
- **Small pull requests, reviewed by humans.** They are easier to reason about, and much easier to roll back at 2am.

<!-- Edit the list above to match how your teams actually work. It reads as
     credible only while it is true, and engineers can tell the difference. -->

## Come build with us

We are hiring engineers across Europe, in teams working on payments, banking, data, and the platform underneath all of it.

**[See open roles →](https://jobs.ashbyhq.com/teya)**

<p align="center">
  <sub>Made by the engineers at <a href="https://www.teya.com">Teya</a>.</sub>
</p>
