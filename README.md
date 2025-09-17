# web3-learning-depth
Learning Web3 Engineering in Details - No slacking of this path till I am fully Decentralized.

---

# 🗓️ 60-Day Web3 Tech Support Engineering Plan

---

## **Week 1 – Blockchain & Web3 Fundamentals (Part 1)**

📌 Goal: Understand blockchain basics and set up tools.

* **Day 1:** Learn blockchain basics → [Ethereum.org Intro](https://ethereum.org/en/developers/docs/intro-to-ethereum/)
* **Day 2:** Install MetaMask, connect to Sepolia testnet → [MetaMask Docs](https://support.metamask.io/)
* **Day 3:** Deploy a simple **ERC-20 contract** on Sepolia using Remix → [Remix IDE](https://remix.ethereum.org/)
* **Day 4:** Use [Etherscan](https://sepolia.etherscan.io/) to check your transaction.
* **Day 5:** Explore **ERC-721 NFT** standard, mint a test NFT.
* **Day 6:** Install `ethers-rs` and fetch ETH balance → [ethers-rs docs](https://docs.rs/ethers/latest/ethers/)
* **Day 7:** Write doc: “How to check your transaction on Etherscan”.

---

## **Week 2 – Blockchain & Web3 Fundamentals (Part 2)**

📌 Goal: Work with Rust Web3 libraries & dApp debugging.

* **Day 8:** Query balances with `ethers-rs` CLI example.
* **Day 9:** Call smart contract function using `ethers-rs`.
* **Day 10:** Explore **The Graph** and query a subgraph. → [The Graph Docs](https://thegraph.com/docs/)
* **Day 11:** Learn common support issues: stuck TX, gas errors.
* **Day 12:** Debug contract call failures, reproduce in Remix.
* **Day 13:** Explore JSON-RPC API (`eth_blockNumber`, `eth_getBalance`). → [Ethereum JSON-RPC Spec](https://ethereum.org/en/developers/docs/apis/json-rpc/)
* **Day 14:** Write support doc: “Why is my transaction pending?”.

---

## **Week 3 – Actix Web & Rust API Development (Part 1)**

📌 Goal: Build a support-facing backend in Rust.

* **Day 15:** Scaffold Actix Web API (`cargo new`). → [Actix Web Book](https://actix.rs/docs/)
* **Day 16:** Add `/` route → returns `"Hello Web3"`.
* **Day 17:** Add `/balance/{address}` → fetch ETH balance via `ethers-rs`.
* **Day 18:** Add `/reverse-ip` route → use SQLite with `sqlx`.
* **Day 19:** Add `/healthz` route.
* **Day 20:** Add `/metrics` route with `prometheus` crate. → [Prometheus Rust crate](https://crates.io/crates/prometheus)
* **Day 21:** Write doc: “Exposing metrics from an Actix Web app”.

---

## **Week 4 – Actix Web & Rust API Development (Part 2)**

📌 Goal: Make the app production-ready.

* **Day 22:** Add middleware (logging, CORS).
* **Day 23:** Add error handling (custom errors).
* **Day 24:** Write integration tests for routes.
* **Day 25:** Add Dockerfile for Actix app.
* **Day 26:** Run container locally → `docker run -p 5000:5000`.
* **Day 27:** Add `docker-compose.yml` for local dev.
* **Day 28:** Write doc: “Running Actix Web in Docker”.

---

## **Week 5 – Infra: Kubernetes & Monitoring (Part 1)**

📌 Goal: Deploy Actix app to Kubernetes.

* **Day 29:** Install Minikube or use GKE. → [Minikube Docs](https://minikube.sigs.k8s.io/docs/start/)
* **Day 30:** Write K8s `Deployment` + `Service` for Actix app.
* **Day 31:** Test with `kubectl port-forward`.
* **Day 32:** Add Prometheus Operator → [prometheus-community/helm-charts](https://github.com/prometheus-community/helm-charts).
* **Day 33:** Configure ServiceMonitor for `/metrics`.
* **Day 34:** Install Grafana with Helm. → [Grafana Helm Chart](https://github.com/grafana/helm-charts)
* **Day 35:** Write doc: “How to scrape Actix Web metrics with Prometheus”.

---

## **Week 6 – Infra: Kubernetes & Monitoring (Part 2)**

📌 Goal: Add monitoring and practice troubleshooting.

* **Day 36:** Deploy node-exporter for node metrics.
* **Day 37:** Build Grafana dashboard for Actix app.
* **Day 38:** Add alerts in Prometheus (high error rate).
* **Day 39:** Simulate pod crash (bad env var), debug with `kubectl logs`.
* **Day 40:** Simulate CrashLoopBackoff (missing dep), debug.
* **Day 41:** Simulate node-exporter Pending issue.
* **Day 42:** Write support doc: “Debugging apps in Kubernetes”.

---

## **Week 7 – Support Simulation & Advanced Troubleshooting**

📌 Goal: Act like a support engineer.

* **Day 43:** Answer mock ticket: “Why is my transaction out of gas?”
* **Day 44:** Mock ticket: “My Prometheus is not scraping metrics.”
* **Day 45:** Mock ticket: “Why is my K8s pod Pending?”
* **Day 46:** Debug Service types (ClusterIP vs NodePort vs LB).
* **Day 47:** Debug “Refused to connect” issues (firewall, Service).
* **Day 48:** Compare **Actix Web vs Flask** performance.
* **Day 49:** Write FAQ: “Common Web3 Support Issues”.

---

## **Week 8 – Final Project & Interview Prep**

📌 Goal: Showcase full-stack support readiness.

* **Day 50:** Build final Actix app with `/balance`, `/reverse-ip`, `/metrics`.
* **Day 51:** Containerize and deploy to GKE.
* **Day 52:** Expose via LoadBalancer service.
* **Day 53:** Set up Prometheus + Grafana dashboards.
* **Day 54:** Add monitoring alerts.
* **Day 55:** Write **support docs** in repo:

  * Setup guide
  * Troubleshooting guide
  * Metrics guide
* **Day 56:** Mock interview: explain app architecture.
* **Day 57:** Mock interview: explain troubleshooting steps.
* **Day 58:** Mock interview: explain ERC-20 vs ERC-721.
* **Day 59:** Mock interview: explain K8s Service types.
* **Day 60:** Final review, polish repo, prepare portfolio/demo.

---

# 🎯 Deliverables by Day 60

✅ Actix Web app with `/balance`, `/reverse-ip`, `/healthz`, `/metrics`.
✅ Dockerized & deployed to Kubernetes (GKE or Minikube).
✅ Prometheus + Grafana monitoring with node-exporter.
✅ Repo with **docs, manifests, support guides**.
✅ Mock interview readiness + troubleshooting confidence.

---

⚡ Commitment: Each week, I will commit code/docs to GitHub so you build a **public portfolio** — to give myself the joy *seeing progress*.

---