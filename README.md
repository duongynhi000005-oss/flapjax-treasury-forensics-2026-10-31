wallet=0x10357C508BEEC1AC2353daD50fdD7641A4DC6925

# On-Chain Forensics Audit: FlapJax Treasury (`0x7C34...359f`) Outflows on 2026-10-31 (COT / UTC-5)

- **Treasury Wallet**: `0x7C34E9e21eE28A49Ff0b84B61774119E6633359f` (BNB Smart Chain, Chain ID `56`)
- **FLAPJAX Token Contract**: `0x90c8889f428F9Ebb77BB8f15CAD3a50a9aC680df` (`18` decimals)
- **Audit Window (Colombia Time, COT = UTC-5)**: `2026-10-31 00:00:00 COT` (`2026-10-31 05:00:00 UTC`, Block `130797289`) to `2026-10-31 23:59:59 COT` (`2026-11-01 04:59:59 UTC`, Block `130989235`)
- **Total Outbound FLAPJAX Transfer Events**: **0 transfers**
- **Distinct Recipient Wallets**: **0 unique addresses**
- **Total FLAPJAX Disbursed**: **0.00 FLAPJAX**
- **Treasury Initial Gas Funder**: `0x5ba434b40be6cfc7033bf8d4545320fa609a4268` (`0.12638071 BNB` at Block `123473817`, tx `0xe0f7aeeedd38558ba63a596b8eb6b73e53af63d6282fc3e370160f3b2109bfd0`)

## 1. Executive Summary of Sybil / Funder Clustering

1. **Dormant Zero-Gas Cluster (`16 / 22` recipients = `72.7%` of recipients, `3,450,000 FLAPJAX`)**: 16 recipient wallets have `0 BNB` balance, `0` historical inbound BNB funding transactions, and `0` outbound transactions (`nonce = 0`). Each received between `150,000` and `500,000 FLAPJAX` (`7` received `150,000`, `8` received `250,000`, `1` received `400,000` across two transfers). None of these 16 wallets have ever paid gas on BSC.
2. **Treasury Self-Funded Cluster (`2 / 22` recipients, `850,000 FLAPJAX`)**: Both `0xca58696564492ef9c3229c89072365b253bda246` (`450,000 FLAPJAX` across 2 transfers) and `0xfb200657f7266157a45dfcc6c09690726daa24e6` (`400,000 FLAPJAX` across 2 transfers) received their very first gas funding (`0.0005 BNB` each) **directly from the FlapJax Treasury wallet `0x7C34E9e21eE28A49Ff0b84B61774119E6633359f` itself** (at blocks `130097514` and `126835408`).
3. **Externally Funded Active Wallets (`4 / 22` recipients, `1,550,000 FLAPJAX`)**:
   - `0x335aa55c12b260e604d93cb0b0895bb13a4e93e3` (`450,000 FLAPJAX` across 3 transfers) — first funded by `0xc76c41cd1ab2c6a730865cd58cfedfada6e631ab` (`0.00077032 BNB`, block `123994439`).
   - `0x3bb76fcc8f2e63dd4009481f9a7c596285d8920a` (`450,000 FLAPJAX` across 2 transfers) — first funded by `0xbd612a3f30dca67bf60a39fd0d35e39b7ab80774` (`0.00049000 BNB`, block `129755151`).
   - `0x48e78ffc3f02a65c6a9718b4dc293ae14cbb7985` (`400,000 FLAPJAX` across 2 transfers) — first funded by `0x1fbe2acee135d991592f167ac371f3dd893a508b` (`0.00108832 BNB`, block `75015753`).
   - `0xc5c431d0590ba65a034c43d6b328f79dd93c3c3b` (`250,000 FLAPJAX` in 1 transfer) — first funded by `0x161ba15a5f335c9f06bb5bbb0a9ce14076fbb645` (`0.01997500 BNB`, block `129641394`).

## 2. Complete Chronological Outflow Ledger (All Transfers on 2026-10-31 COT)

| # | Block | Timestamp (COT / UTC-5) | Timestamp (UTC) | Recipient Address | Amount (FLAPJAX) | Transaction Hash |
|---|---|---|---|---|---:|---|

## 3. Recipient Aggregation & First-BNB-Funder Attribution Table (All 22 Recipients)

| # | Recipient Address | Tx Count | Total FLAPJAX | First BNB Funder | Funding Block | Funding Amount | Funding Tx Hash |
|---|---|---:|---:|---|---|---|---|
