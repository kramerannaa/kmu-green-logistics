# KMU Nachhaltige Lieferketten & Green Logistics
### ExInt II | WU Vienna | SS 2026 | Anna Kramer

## Research Question
Wie integrieren exportorientierte KMU Nachhaltigkeitsziele in ihre internationalen
Supply-Chain-Entscheidungen, und welche institutionellen sowie ressourcenbedingten
Faktoren beeinflussen diesen Prozess?

## Hypotheses
- **H1:** Regulatorischer Druck (CSRD, CBAM, CSDDD) erhöht die Adoption
  nachhaltiger Logistikpraktiken bei exportorientierten KMU.

## Theoretical Foundation
**Institutional Theory (DiMaggio & Powell, 1983):**
Regulativer Druck (CSRD, CBAM, CSDDD), normativer Druck (Kundenerwartungen
aus Lieferketten) und mimetischer Druck zwingen KMU zur Adoption
nachhaltiger Logistikpraktiken.

**Resource-Based View (Barney, 1991):**
Die Fähigkeit zur Umsetzung hängt von internen Ressourcen ab — finanzielle,
personelle und informationelle Kapazitäten bestimmen, ob KMU auf
institutionellen Druck substanziell oder nur symbolisch reagieren.

## Variables

### Dependent Variable (Y)
| Construct | Data Item(s) | Formula |
|-----------|-------------|---------|
| RoA | nicon, at | nicon / at |
| EBITDA | ebitda | direct field |
| Sales Growth | sale | (sale_t - sale_t-1) / sale_t-1 |

### Independent Variable (X)
| Construct | Data Item(s) | Formula |
|-----------|-------------|---------|
| R&D Intensity | xrd, at | xrd / at |
| Capital Expenditure | capx, at | capx / at |

### Controls
| Construct | Data Item(s) | Formula |
|-----------|-------------|---------|
| Firm Size | at | log(at) |
| Leverage | dltt, dlc, seq | (dltt+dlc) / seq |
| Employees | emp | direct field |
| Cash Holdings | che, at | che / at |
| Tangibility | ppent, at | ppent / at |
| Total Assets | at | direct field |
| Total Liabilities | lt | direct field |
| Revenue | sale | direct field |
| Operating Income | oiadp | direct field |
| Depreciation | dp | direct field |
| Interest Expense | xint | direct field |
| Cash Flow Operations | oancf | direct field |
| Long-term Debt | dltt | direct field |
| Short-term Debt | dlc | direct field |
| Stockholders Equity | seq | direct field |
| Retained Earnings | re | direct field |
| Inventory | invt | direct field |
| Accounts Receivable | rect | direct field |
| Accounts Payable | ap | direct field |
| Current Assets | act | direct field |
| Current Liabilities | lct | direct field |
| Pretax Income | pi | direct field |
| Income Taxes | txt | direct field |
| SGA Expense | xsga | direct field |
| Cost of Goods Sold | cogs | direct field |
| Staff Expense | xlr | direct field |
| Intangible Assets | intan | direct field |
| Goodwill | gdwl | direct field |
| Working Capital | wcap | direct field |
| Gross Profit | revt, cogs | revt - cogs |
| Net Income | nicon | direct field |

## Data
- Source: WRDS / Compustat Global (g_funda)
- Sample: Österreichische exportorientierte KMU (≤250 Mitarbeiter, loc=AUT)
- Zeitraum: 2015-2024

## How to Reproduce
git clone https://github.com/kramerannaa/kmu-green-logistics
python3 -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
task all

## Data Provenance
| Item | Detail |
|------|--------|
| Source | WRDS / Compustat Global |
| Table | comp_global_daily.g_funda |
| Downloaded | 2026-05-28 |
| License | WRDS subscriber agreement |
| Fiscal years | 2015-2024 |
| Raw rows | 338,462 |
| Clean rows | 26,090 |

## Data Provenance
| Item | Detail |
|------|--------|
| Source | WRDS / Compustat Global |
| Table | comp_global_daily.g_funda |
| Downloaded | 2026-05-28 |
| License | WRDS subscriber agreement |
| Fiscal years | 2015-2024 |
| Raw rows | 338,462 |
| Clean rows | 26,090 |
