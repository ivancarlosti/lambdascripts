# Lambda scripts

Scripts for Lambda actions to be called by n8n

<!-- buttons -->
[![Stars](https://img.shields.io/github/stars/ivancarlosti/awssesconverter?label=⭐%20Stars&color=gold&style=flat)](https://github.com/ivancarlosti/awssesconverter/stargazers)
[![Watchers](https://img.shields.io/github/watchers/ivancarlosti/awssesconverter?label=Watchers&style=flat&color=red)](https://github.com/sponsors/ivancarlosti)
[![Forks](https://img.shields.io/github/forks/ivancarlosti/awssesconverter?label=Forks&style=flat&color=ff69b4)](https://github.com/sponsors/ivancarlosti)
[![GitHub commit activity](https://img.shields.io/github/commit-activity/m/ivancarlosti/awssesconverter?label=Activity)](https://github.com/ivancarlosti/awssesconverter/pulse)
[![GitHub Issues](https://img.shields.io/github/issues/ivancarlosti/awssesconverter?label=Issues&color=orange)](https://github.com/ivancarlosti/awssesconverter/issues)
[![License](https://img.shields.io/github/license/ivancarlosti/awssesconverter?label=License)](LICENSE)  
[![GitHub last commit](https://img.shields.io/github/last-commit/ivancarlosti/awssesconverter?label=Last%20Commit)](https://github.com/ivancarlosti/awssesconverter/commits)
[![Security](https://img.shields.io/badge/Security-View%20Here-purple)](https://github.com/ivancarlosti/awssesconverter/security)
[![Code of Conduct](https://img.shields.io/badge/Code%20of%20Conduct-2.1-4baaaa)](https://github.com/ivancarlosti/awssesconverter?tab=coc-ov-file)
[![GitHub Sponsors](https://img.shields.io/github/sponsors/ivancarlosti?label=GitHub%20Sponsors&color=ffc0cb)][sponsor]
[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-ffdd00)][buymeacoffee]
<!-- endbuttons -->

# Configuration

* Runtime: Python 3.13+
* Architectune: arm64/x86_64 (arm64 is cheaper)
* Timeout: 1 minute
* Requires related policy for each script

# Instruction

* Create function using `.py` code 
* Configure as specified below
* Attach related `.json` policy  on function's role

# Remote call instruction

* Create an IAM user for remote function execution
* Attach related `remotecall_policy_lambda.json` policy on user

# Notes

* AddTag script uses Alias to tag KMS keys
* AddTag script uses Description to tag Route53 zones
* Backup Alert script uses 1 day as range window to gather fails and expired alerts
* Billing and AddTag scripts uses "Tenant" tag set resources

<!-- footer -->
---

## 🧑‍💻 Consulting and technical support
* For personal support and queries, please submit a new issue to have it addressed.
* For commercial related questions, please [**contact me**][ivancarlos] for consulting costs. 

| 🩷 Project support |
| :---: |
If you found this project helpful, consider [**buying me a coffee**][buymeacoffee]
|Thanks for your support, it is much appreciated!|

[cc]: https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-code-of-conduct-to-your-project
[contributing]: https://docs.github.com/en/articles/setting-guidelines-for-repository-contributors
[security]: https://docs.github.com/en/code-security/getting-started/adding-a-security-policy-to-your-repository
[support]: https://docs.github.com/en/articles/adding-support-resources-to-your-project
[it]: https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/configuring-issue-templates-for-your-repository#configuring-the-template-chooser
[prt]: https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/creating-a-pull-request-template-for-your-repository
[funding]: https://docs.github.com/en/articles/displaying-a-sponsor-button-in-your-repository
[ivancarlos]: https://ivancarlos.me
[buymeacoffee]: https://buymeacoffee.com/ivancarlos
[paypal]: https://icc.gg/donate
[sponsor]: https://github.com/sponsors/ivancarlosti
