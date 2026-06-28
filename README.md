# Ping GPMS Shadowrocket Ad Rules

Shadowrocket rules extracted from `p_ping_gpms_apk_0a8cfea2718f91187b748ecf4691a2bf.apk`.

- APK SHA256: `8d11bc1001d2bee0e09afe17254d59f00f6d04ea37435075a3db8442a6a7c7b8`
- APK size: `81451971` bytes
- Analysis date: `2026-06-29`
- Rule file: `shadowrocket-adblock.list`

## Use

Add this raw URL as a Shadowrocket remote rule set:

```text
https://raw.githubusercontent.com/Lincoln233/ping-gpms-shadowrocket-rules/main/shadowrocket-adblock.list
```

## Method

Static extraction from APK DEX/resources/assets/native strings. The final list keeps ad, bid, SSP, ad SDK config, ad SDK CDN, and ad SDK telemetry domains tied to embedded SDKs such as AnyThink/TopOn, Pangle, Kuaishou Ads, Sigmob, UC/Noah, Baidu/Huichuan, iQIYI Cupid, Tanx/Alimama, Wangmai, and Umeng telemetry.

Obvious auth, payment, app API, generic certificate, SVG, and source-code documentation domains were excluded.

## Files

- `shadowrocket-adblock.list`: Shadowrocket `DOMAIN-SUFFIX,...,REJECT` rules.
- `domains.txt`: plain domain list.
- `evidence.tsv`: selected domain evidence from APK strings.
