# popdock-web-eqa-dryrun

Public orchestrator only. It runs a stubbed EQA-style build against private
`stokedconsulting` copies of Popdock.Web and siblings.

It does not contain product source. It does not touch `eonesolutions`.
It does not deploy to EQA or production. Azure deploy is skipped; success
is `publish_output/Popdock.Web.dll` as an Actions artifact.

Private repos in this org cannot start GitHub Actions jobs (Free plan,
`startup_failure` / 0 jobs). Public repos can. That is why this workflow
lives here instead of inside `stokedconsulting/Popdock.Web`.
