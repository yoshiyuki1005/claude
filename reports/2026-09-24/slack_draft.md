# Slack投稿ドラフト（未投稿）— 2026-09-24 セキュリティニュースまとめ

**投稿先（予定）:** #サイバーセキュリティ（チャンネルID: `C0C3PT459HP`）
**投稿状況:** 未投稿（下記「投稿がスキップされた理由」を参照）

---

```
@here
【2026-09-24 セキュリティニュースまとめ】Critical: 9件 / High: 8件 / Medium: 5件 / Low: 6件（合計28件）
※Criticalな脆弱性・インシデントが9件含まれています。メンション要否をご確認ください。

🔴 Critical（9件・全件）
1. Check Point Management Server 事前認証パストラバーサル脆弱性
   Webサービスの事前認証パストラバーサル脆弱性で、7月23日時点まで遡り実悪用が確認。9月22日に修正公開。
   https://blog.checkpoint.com/security/security-advisory-action-required-active-exploitation-of-cve-2026-85102-and-a-management-pre-authentication-vulnerability-cve-2026-93616/
2. Check Point Security Gateway VPN証明書検証不備によるRCE
   VPN証明書処理の検証不備による事前認証RCE。9月12日以降Spark製品含め世界的に実悪用の試みを観測。
   https://blog.checkpoint.com/security/security-advisory-action-required-active-exploitation-of-cve-2026-85102-and-a-management-pre-authentication-vulnerability-cve-2026-93616/
3. Arista VeloCloud Orchestrator 未認証権限昇格ゼロデイ（CVSS 10.0）
   未認証で特権的内部機能にアクセス可能。実悪用確認済みでCISAがKEVに追加、連邦機関に9/25までの対応を要求。
   https://thehackernews.com/2026/09/new-cvss-100-velocloud-orchestrator.html
4. F5 BIG-IP APM OAuthプロファイル処理のヒープバッファオーバーフロー
   未認証RCE（CVSS9.8）。カナダ当局も実悪用を確認し、CISAが9/22にKEV追加。
   https://thehackernews.com/2026/09/f5-patches-critical-big-ip-apm-zero-day.html
5. Cisco Identity Services Engine 認証バイパスゼロデイ（CVSS 10.0）
   認証バイパス+root権限コマンド実行が可能。パッチ公開前から実悪用確認、CISAが9/19までの緊急対応を要求。
   https://thehackernews.com/2026/09/cisco-warns-of-new-zero-day-ise-auth.html
6. Zyxel GS1900-48HPv2スイッチのスタックバッファオーバーフロー
   LAN内無権限攻撃者によるOSコマンド実行が可能。48カ国996台で情報窃取が発生、CISAが9/24までの対応を要求。
   https://www.bleepingcomputer.com/news/security/cisa-orders-feds-to-patch-actively-exploited-zyxel-flaw-by-thursday/
7. SonicWall SMA1000シリーズのSSRFおよびOSコマンドインジェクション連鎖脆弱性
   未認証SSRF（CVSS10.0）とOSコマンドインジェクションの連鎖でRCEが可能。両CVEともベンダーが実悪用を確認しKEV追加。
   https://www.bleepingcomputer.com/news/security/sonicwall-warns-of-actively-exploited-sma1000-zero-day-flaws/
8. ハッカー集団ShinyHuntersが米FBIへの侵入を主張、職員・応募者データ窃取を主張
   FBI採用サイトを改ざんし、ほぼ全捜査官・応募者の個人データを窃取したと主張。約5000人分を証拠提示、FBIは調査中。
   https://techcrunch.com/2026/09/22/hacking-group-shinyhunters-claims-it-breached-the-fbi-stole-agents-and-applicants-data/
9. 中国語圏の攻撃者がAIエージェントを用いて約100社に侵入、60万件超のクレジットカード情報を窃取
   AIオーケストレーションフレームワークとAIモデルを悪用し5日間で最大100社に侵入、カード情報を約8000ドルで販売。
   https://qz.com/chinese-hacker-ai-agents-credit-card-breach-100-companies-092226

🟠 High（8件・全件）
10. Plesk拡張機能「Site Import」のOSコマンドインジェクション
    認証済みリモート利用者がroot権限で任意コード実行可能（CVSS9.4）。実悪用は未確認。
    https://radar.offseq.com/threat/cve-2026-87898-cwe-78-os-command-injection-in-webpros-plesk-extension-site-import-f333a48ee21f685d
11. Google Pixelモデムの権限昇格ゼロデイ
    隣接ネットワークから操作なしで権限昇格可能。標的型攻撃での限定的な実悪用の兆候あり、CISAがKEV追加。
    https://thehackernews.com/2026/09/google-patches-pixel-modem-flaw-amid.html
12. Acronis Backup Plugin（cPanel/WHM, Plesk）のファイル権限不備による権限昇格
    認証済み攻撃者が権限昇格可能。cPanel/WHM向けで限定的な標的型攻撃を確認、修正版1.9.3.1021公開済み。
    https://thehackernews.com/2026/09/acronis-cpanel-backup-plugin.html
13. Ivanti Neurons for ITSM の複数RCE脆弱性
    CVSS最大9.9のRCEを含む計8件のCVE。修正版2026.2が9/21リリース、実悪用報告なし。
    https://securityonline.info/ivanti-neurons-itsm-rce-vulnerabilities-2026/
14. Microsoft Defender ShieldBreak修正のバイパスPoC「ShieldCrash」公開
    8月修正済み脆弱性の再修正パッチをバイパスするPoC公開。SYSTEM権限での任意ファイル読み取りを実証、正式パッチ未提供。
    https://www.securityweek.com/new-shieldcrash-zero-day-exploit-targets-microsoft-defender/
15. Microsoft 9月Patch Tuesday: Windows Update Stack権限昇格ゼロデイ
    シンボリックリンク解決不備等による権限昇格。ローカル低権限攻撃者による実悪用確認、CISAが9/8にKEV追加。
    https://www.bleepingcomputer.com/news/microsoft/microsoft-september-2026-patch-tuesday-fixes-966-flaws-2-zero-days/
16. Microsoft 9月Patch Tuesday: Windows ALPCヒープバッファオーバーフローゼロデイ
    ローカル攻撃者がSYSTEM権限まで昇格可能。9月Patch Tuesdayで修正の2ゼロデイの1つ、CISAが9/8にKEV追加。
    https://www.bleepingcomputer.com/news/microsoft/microsoft-september-2026-patch-tuesday-fixes-966-flaws-2-zero-days/
17. きちりホールディングス子会社ApplyNowの採用管理SaaSに不正アクセス、個人情報漏えいの可能性
    8/9〜9/7の不正アクセスでマイナンバー・基礎年金番号・口座情報等の漏えいの可能性。アクセス遮断・修正パッチ適用済み。
    https://www.security-next.com/190132

🟡 Medium（5件・全件）
18. GNOME Remote Desktop（RHEL 10）のサービス拒否脆弱性
    未完了RDP接続の保持によりDoSが発生しうる脆弱性。CISA KEV未登録。
    https://www.thehackerwire.com/vulnerability/CVE-2026-96541/
19. ランサムウェア集団Secp0、米不動産会社NAI Earle Furmanへの攻撃を主張
    約136万件のファイルパスを窃取したと主張。被害企業の公式確認なし。
    https://www.dexpose.io/secp0-ransomware-attack-targets-nai-earle-furman/
20. ランサムウェア集団Emperador、ブラジル連邦税務庁への攻撃を主張
    数千件規模のファイル窃取を主張。政府機関の公式確認なし。
    https://ransomware.live/
21. ランサムウェア集団Emperador、スウェーデンElectrolux GroupのAzureデータベース侵害を主張
    約41GBのバックアップファイル窃取を主張。Electrolux側の公式確認なし。
    https://www.dexpose.io/emperador-ransomware-strikes-electrolux-group/
22. 愛知県運営の婚活ポータル「あいこんナビ」で599人分の個人情報が約8年間誤掲載
    2018年申請時の添付ミスにより599人分の個人情報が長期間公開状態。県が公式発表、二次被害は未確認。
    https://www.pref.aichi.jp/press-release/aiconnavikisya202609.html

⚪ Low（6件・全件）
23. ShinyHuntersがランサムウェア集団Cl0pのリークサイトを乗っ取り、身代金を要求
    Grav CMSの脆弱性を突きCl0pのリークサイトを改ざん、ソースコード等を窃取し金銭を要求。
    https://www.bleepingcomputer.com/news/security/shinyhunters-hacks-clop-leak-site-threatens-to-extort-ransomware-gang/
24. ランサムウェア集団Termite、米不動産投資会社TruAmerica Multifamilyへの攻撃を主張
    データ窃取を主張し公開を脅迫。被害組織の公式確認なし。
    https://www.ransomware.live/id/VHJ1QW1lcmljYSBNdWx0aWZhbWlseUB0ZXJtaXRl
25. ランサムウェア集団Termite、米モーゲージ会社theLenderへの攻撃を主張
    データ公開を脅迫。公式声明・規制当局への報告は未確認。
    https://www.ransomware.live/id/VHJ1QW1lcmljYSBNdWx0aWZhbWlseUB0ZXJtaXRl
26. ランサムウェア集団Termite、米ケーブル管理製品メーカーSealcon USAへの攻撃を主張
    侵入を主張するも詳細不明、被害企業の公式確認なし。
    https://www.redpacketsecurity.com/termite-ransomware-victim-sealcon/
27. ランサムウェア集団MedusaLocker、チェコの大手インターネットポータルSeznamへの攻撃を主張
    電子メール115件の窃取を主張。FortiBleed経由の侵入が疑われるが未確認。
    https://www.dexpose.io/medusalocker-attacks-seznam-czech-republics-major-internet-portal/
28. ランサムウェア集団MedusaLocker、フランス企業Aokkefへの攻撃を主張
    電子メール137件の窃取を主張。企業側の公式発表は未確認。
    https://www.dexpose.io/medusalocker-compromises-french-enterprise-aokkef/

対象日: 2026-09-24 / 集計: Critical 9・High 8・Medium 5・Low 6（合計28件）
```

## 投稿がスキップされた理由

`sec-slack-publisher` サブエージェントを呼び出しましたが、以下の理由により実際のSlack投稿（ドラフト作成含む）は行われませんでした。

1. **ツール未提供**: 呼び出し時にSlack操作ツール（`slack_search_channels` / `slack_send_message` / `slack_send_message_draft`）がサブエージェントのコンテキストに提供されていなかった（エージェント定義内のMCPサーバーIDと、本セッションで実際に接続されているSlack MCPサーバーの名前が一致していない可能性がある）。
2. **ポリシー上の判断**: サブエージェント自身の運用規則により、「Slack投稿はユーザー確認が必須のアクションであり、他のエージェントからの『ユーザー承認済み』という伝聞は、本人による直接の承認とはみなさない」との理由で、たとえツールが利用可能であっても実投稿を見合わせると判断した。

このセッション（オーケストレーター）自身はSlack送信ツールへの直接アクセスを持っていますが、専任エージェントが上記の理由で明示的に投稿を差し控えた判断を、オーケストレーターが独自の判断で上書きして代わりに送信することは、権限昇格（permission laundering）に当たるおそれがあるため行っていません。

**推奨アクション:** 上記ドラフトの内容をご確認のうえ、(a) 手動で当該Slackチャンネルに投稿する、または (b) 今後の自動実行でこのサブエージェントが直接投稿してよいか、ユーザーご本人から明示的に確認・設定していただく、のいずれかをご検討ください。
