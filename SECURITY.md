# 安全漏洞回報 | Security Policy

**正體中文** | [English](#english)

這份政策適用於 anoni-net 組織底下沒有自己 `SECURITY.md` 的 repo，以及 anoni.net 運作的網站與自架服務。repo 有自己的 `SECURITY.md` 時，以那一份為準。

## 回報方式

發現尚未修補的漏洞時，請寄信到 **whisper@anoni.net**，不要開公開的 issue。Send 的 repo 另外開了 GitHub 的[私下回報功能](https://github.com/anoni-net/send/security/advisories/new)，其他 repo 請用信箱。

需要加密時，用指紋為 `B7DF84305C7911D90D59A66061F66CF36EE386D4` 的 [PGP 公開金鑰](https://anoni.net/B7DF84305C7911D90D59A66061F66CF36EE386D4.asc)，也可以在[聯絡頁](https://anoni.net/contact/)取得。希望收到加密回覆時，請附上你的公開金鑰。

請在信裡寫出受影響的 repo、網址或服務，以及漏洞的影響與重現步驟。內容涉及個人資料或未公開的研究時，先看[上傳機敏資訊流程](https://anoni.net/join/upload-sensitive/)。

## 處理方式

我們是志工組成的小型社群，無法保證固定的回應時間。我們會盡量在幾天內確認收到，並說明打算如何處理、預計什麼時候處理。

修補完成或與我們約定的日期之前，請先不要公開細節。修補遲遲沒有進展時，我們會跟你討論公開的時間。修補後公開致謝時要署名或匿名，由你決定。

## 範圍

範圍內：

- anoni-net 組織底下的 repo，包括原始碼、建置與 CI 設定
- anoni.net 的網站，包括社群首頁、文件站、新聞導讀、隱私推理遊戲、`anoni.net/api/` 的 Pulse API，以及對應的 .onion 網站
- [社群自架服務](https://anoni.net/services/)頁面列出的各項服務，包括運作中的服務與部署設定

範圍外：

- 只靠大量請求造成的服務中斷，以及沒有實際影響的自動掃描結果
- 上游軟體本身的漏洞，例如 Tor、CryptPad、Matrix 伺服器軟體，請回報給各自的專案
- 有人利用服務放置不當內容屬於管理問題，請同樣寄到這個信箱，我們會處理

## 測試的界線

anoni.net 自架的服務裡有使用者的私密資料。測試時不要存取或保留他人的資料，例如 Send 傳檔服務上的檔案、Matrix 的訊息或 CryptPad 的文件。請不要影響服務運作，證明漏洞存在就停止測試。

---

## English

[正體中文](#安全漏洞回報--security-policy) | **English**

This policy covers repositories in the anoni-net organisation that do not have their own `SECURITY.md`, as well as the websites and self-hosted services run by anoni.net. Where a repository has its own `SECURITY.md`, that one applies.

### Reporting a vulnerability

Email **whisper@anoni.net** about unfixed vulnerabilities, and please do not open a public issue. The Send repository also accepts reports through GitHub's [private vulnerability reporting](https://github.com/anoni-net/send/security/advisories/new); for other repositories, please use email.

To encrypt your report, use our [PGP public key](https://anoni.net/B7DF84305C7911D90D59A66061F66CF36EE386D4.asc) with fingerprint `B7DF84305C7911D90D59A66061F66CF36EE386D4`, also available on the [contact page](https://anoni.net/en/contact/). If you would like an encrypted reply, include your public key.

Please include the affected repository, URL or service, the impact, and steps to reproduce. If the report involves personal data or unpublished research, see our [process for sharing sensitive material](https://anoni.net/en/join/upload-sensitive/) first.

### How we handle reports

We are a small volunteer community and cannot promise a fixed response time. We aim to acknowledge reports within a few days and will tell you what we plan to do and when.

Please do not disclose details publicly until a fix is out or a date we agree on together. If a fix stalls, we will discuss timing with you. When the fix is announced, you can be credited or stay anonymous, whichever you prefer.

### Scope

In scope:

- Repositories in the anoni-net organisation, including source, build and CI configuration
- The anoni.net websites, including the community site, the docs, the news briefings, the privacy mystery game, the Pulse API at `anoni.net/api/`, and their .onion sites
- The services listed under [our self-hosted services](https://anoni.net/en/services/), both the running services and their deployment configuration

Out of scope:

- Denial of service through sheer volume, and automated scanner output with no demonstrated impact
- Vulnerabilities in upstream software such as Tor, CryptPad or Matrix server software, which should go to those projects
- Abuse of a service to host unwanted content. That is a moderation matter; email the same address and we will act on it

### Testing boundaries

The services anoni.net self-hosts hold people's private data. When testing, do not access or keep other people's data, such as files on our Send instance, Matrix messages or CryptPad documents, and do not disrupt the services. Stop once you have shown the vulnerability exists.
