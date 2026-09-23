:shield: *サイバーセキュリティニュース日次まとめ（2026-09-22）*
対象期間: 直近24〜48時間中心（脆弱性/インシデント）、直近1週間（規制/技術トレンド）｜全34件（Critical 7 / High 7 / Medium 13 / Low 7）

━━━━━━━━━━━━━━━━━━
:red_circle: *Critical（7件）* — 実悪用確認・影響範囲が広いもの
━━━━━━━━━━━━━━━━━━

1. *<https://thehackernews.com/2026/09/cisco-warns-of-new-zero-day-ise-auth.html|Cisco ISE 認証バイパス・ゼロデイ（CVSS 10.0）>*
   未認証でroot権限コマンド実行が可能。CISAが実悪用を確認しKEVへ追加（9/16）。
2. *<https://www.bleepingcomputer.com/news/security/cisco-confirms-cve-2026-20079-secure-fmc-flaw-exploited-in-attacks/|Cisco Secure FMC 認証バイパス（CVSS 10.0）>*
   Sandworm等複数の脅威アクターが悪用。未認証でroot権限奪取。KEV追加済み（9/9）。
3. *<https://www.helpnetsecurity.com/2026/08/21/citrix-netscaler-gateway-cve-2026-19490/|Citrix NetScaler ADC/Gateway 認証バイパス>*
   Gateway/AAA仮想サーバー構成で未認証ログインバイパス。実悪用ありKEV追加（9/9）。
4. *<https://thehackernews.com/2026/09/adobe-patches-magento-zero-day.html|Adobe Commerce/Magento「StyleSmuggler」RCE（CVSS 10.0）>*
   支払い失敗メール生成過程で未認証RCE。実環境での悪用を確認、9/7に緊急パッチ公開。
5. *<https://thehackernews.com/2026/09/cisa-flags-three-linux-kernel.html|Linuxカーネル 複数脆弱性（TLS/ebtables）実悪用確認>*
   CISAが3件をKEVへ追加（9/18）。TLS受信パス・ebtables SNATの不備。
6. *<https://www.theregister.com/security/2026/09/18/north-koreas-fake-job-interviews-infected-30000-devices/5297461|北朝鮮系「WaterPlum」偽採用面接キャンペーン、3万台超感染>*
   日米豪独当局が共同注意喚起。100カ国以上・暗号資産約1070万ドル窃取。
7. *<https://www.bleepingcomputer.com/news/security/centerpoint-energy-confirms-customer-data-stolen-in-cyberattack/|米電力大手CenterPoint Energy、顧客データ流出をSEC提出書類で確認>*
   約749万件（社会保障番号の一部含む）の顧客記録窃取の主張を受け攻撃発生を確認。

━━━━━━━━━━━━━━━━━━
:large_orange_circle: *High（7件）* — PoC公開/限定悪用、対応期限が近い規制等
━━━━━━━━━━━━━━━━━━

1. *<https://www.cisa.gov/news-events/alerts/2026/09/21/cisa-adds-one-known-exploited-vulnerability-catalog|Zyxel GS1900シリーズ バッファオーバーフロー>* — KEV追加、連邦機関は9/24までに対応要求。
2. *<https://thehackernews.com/2026/09/zyxel-and-veeam-flaws-under-active.html|Veeam Agent for Windows 権限昇格>* — PoC公開後、実悪用をArctic Wolfが報告。
3. *<https://vuldb.com/vuln/408026|Netcore NBR200V2ルーター コマンドインジェクション（CVSS 10.0）>* — PoC公開、パッチ未提供。
4. *<https://cybernews.com/news/iran-tanker-cyberattacks-us-ships-monitored/|石油タンカー3隻でサイバー攻撃疑い>* — 米沿岸警備隊・FBIが調査、約20隻を監視。
5. *<https://www.ppc.go.jp/personalinfo/legal/r8kaiseihogohou/|改正個人情報保護法、政令・規則・ガイドライン整備の進め方を決定>* — 課徴金制度導入、2028年7月全面施行予定。
6. *<https://www.freshfields.com/en/our-thinking/blogs/technology-quotient/cyber-resilience-act-reporting-obligations-take-effect-on-11-september-2026-102nzmk|EUサイバーレジリエンス法、脆弱性・インシデント報告義務が発効>* — 24時間/72時間以内の報告義務（9/11発効済み）。
7. *<https://www.cyber.go.jp/law/lawlink.html|サイバー対処能力強化法、10/1本則施行>* — 重要インフラ事業者に侵害事象の報告義務。

━━━━━━━━━━━━━━━━━━
:large_yellow_circle: *Medium（13件）* — 影響限定的・パッチ提供済み等
━━━━━━━━━━━━━━━━━━
• <https://source.android.com/docs/security/bulletin/2026/2026-09-01|Android IMS認証バイパス>（9月更新で修正済み）
• <https://osv.dev/vulnerability/CVE-2026-86462|Apache Airflow FAB providerセッション不備>（3.9.0で修正済み）
• <https://www.securityweek.com/isc-patches-14-vulnerabilities-in-bind-9-security-update/|ISC BIND 9 複数脆弱性>（修正済み、実悪用未確認）
• <https://www.oracle.com/security-alerts/cspusep2026.html|Oracle 2026年9月CPU>（800件超修正）
• <https://securityonline.info/cisco-secure-firewall-vulnerabilities-september-2026/|Cisco Secure Firewall 複数脆弱性>（修正済み、悪用報告なし）
• <https://www.prnewswire.com/news-releases/aecom-data-breach-investigation-edelson-lechtzin-llp-probes-class-action-claims-after-hackers-allege-theft-of-more-than-1-tb-of-data-302884076.html|AECOM、ランサムウェア被害主張>（未確認）
• <https://www.redpacketsecurity.com/metaencryptor-ransomware-victim-beckman-coulter-inc/|Beckman Coulter、ランサムウェア被害主張>（未確認）
• <https://www.ipa.go.jp/security/reports/vuln/kenkyukai-report2026.html|IPA 早期警戒パートナーシップガイドライン改訂案（第14版）>（パブコメ中）
• <https://content.govdelivery.com/accounts/USDHSCISA/bulletins/42b055b|CISA、週次脆弱性速報を廃止しリスクベース管理へ移行>
• <https://www.safelogic.com/blog/what-happens-on-september-21-2026|NIST CMVP、FIPS 140-2認証を全件Historical化>
• <https://docs.opnsense.org/releases/CE_26.7.html|OPNsense 26.7.4リリース>（Suricata/Unbound更新）
• <https://techcommunity.microsoft.com/blog/microsoft-entra-blog/what%E2%80%99s-new-in-microsoft-entra-september-2026/4545179|Microsoft Entra、Security AdministratorロールにID侵害対応機能追加>

━━━━━━━━━━━━━━━━━━
:white_circle: *Low（7件）* — 参考情報
━━━━━━━━━━━━━━━━━━
• <https://www.theregister.com/cyber-crime/2026/09/21/clop-gets-a-taste-of-its-own-medicine-after-shinyhunters-hijack-leak-site/5297702|ShinyHuntersがランサムウェア集団Clopのリークサイトを侵害>
• <https://www.galaxywarden.com/blog/breach/hoyletanner-com-braincipher-2026-09|Hoyle, Tanner & Associates、ランサムウェア被害主張>（未確認）
• <https://www.dexpose.io/incransom-targets-appliance-factory-mattress-kingdom/|Appliance Factory & Mattress Kingdom、ランサムウェア被害主張>（未確認）
• <https://www.galaxywarden.com/blog/breach/diarco-com-ar-incransom-2026-09|アルゼンチンDiarco、ランサムウェア被害主張>（未確認）
• <https://www.nist.gov/news-events/news/2026/07/ai-data-center-security-analysis-draft-sp-800-239-available-public-comment|NIST SP 800-239（AIデータセンターセキュリティ）パブコメ中>
• <https://www.ietf.org/archive/id/draft-bruhns-securitytxt-product-security-00.html|IETF、security.txtに製品セキュリティ用フィールドを提案>
• <https://arxiv.org/abs/2609.12305|説明可能AI異常検知フレームワーク「ExCYDER」提案論文>

━━━━━━━━━━━━━━━━━━
_Generated by sec-vuln-analyst / sec-incident-analyst / sec-policy-analyst / sec-techtrend-analyst → sec-severity-classifier_
