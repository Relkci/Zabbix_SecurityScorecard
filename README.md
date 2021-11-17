# Zabbix_SecurityScorecard
Zabbix Template for Security Scorecard to Monitor your organization, comeptitors, and vendors overall scores

# Installation
- On SecurityScorecard, add three portfolios and add organizations respectively:
  - One to contain your organizations
  - One to contain your competitors
  - One to contain your vendors
- In Zabbix Import template
- Create host, add agent interface
- Assign template
- Set inherited macros (API Key, Alert Thresholds)
- Initial data will take aproximately 2 hours to obtain with discovery rules.
- After Discovery completes, search the items for "Security Scorecard Porfolio YOUR_PORTFOLIO_NAME - ID.
- Copy the IDs for the portfolios containing your organizations, your competitors, and your vendors.
- Updat the inherited macro's that specify the "primary" (your organizations), competitors, and vendors IDs.  
- These will be used to obtain detailed stats for all the organizations within those portfolios.  Data is aggregated and compared to produce % of score across portfoliios.

# Features
- Retrieves Profile IDS
- Retrieves Scorecard summaries for all organizations within primary, compeititor, and vendor portfolios
- Triggers on score thresholds and score drops
- Obtails vendor lists for each organization within the primary, competitor, and vendor portfolios.
- Graphs and Dashboards
 
# LLD Discovery
- Portfolios
- Organizations within portfolios (scores, industry, vendor associations etc)

# Triggers 
- Primary Average Score Portfolio Dropped Below threshold
- Primary Organization Score Dropped Below threshold
- Primary Average Score Drop
- Primary Organization Score Drop
- Primary Average Score as Percent of Competitor Average Score Dropped Below threshold
- Primary Average Score as Percent of Competitor Average Score Dropped

# Dashboards
- Primary Portfolio Dashoard
- Vendor Portfolio Dashboard
- Competitor Portfolio Dashboard

