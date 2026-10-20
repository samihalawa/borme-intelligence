# Detailed source-specific workflow


1. Resolve company identity from the supplied legal name and province, and specify an issue date. Do not confuse similarly named entities. Use registry references or a company identifier in the source to disambiguate where available; a matching name alone is not proof of identity.
2. Run `borme_company_notices` for one date and province. The implementation reads the official Section A province XML and matches company headings, not people mentioned inside notices. It is a bounded issue lookup, not a complete company history or an alerting service. If an issue or province document is unavailable, distinguish that failure from zero matches.
3. Preserve the notice number, company heading, complete act text, publication date, registration details and official document link. Separate the act or registration date from the gazette publication date. Summarize event types without adding undisclosed financial or ownership conclusions.
4. Treat an incorporation, capital change, appointment, resignation, correction, address change or dissolution as a published event. Do not infer solvency, creditworthiness, beneficial ownership, fraud, employment status or suitability for investment from it. Do not compile dossiers about private individuals or harvest personal contact details.
5. Produce a concise event brief and identity limitations. A certification or complete current legal status requires the competent registry. Repeat-date checks are user-initiated unless a separately authorized native scheduler is actually configured.

## Output

Entity identity and confidence; exact issue/province coverage; notice number; act and registration dates; concise event summary; official text links; limits of inference.

