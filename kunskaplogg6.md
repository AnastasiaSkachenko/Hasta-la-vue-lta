## Vecka 43 – Typad end-to-end

**Kursmål:** Fullstack 2 (redogöra för GraphQL – nu klientsidan: cache, och vad en fråga kostar) · Fullstack 11 (implementera ett GraphQL-API – med N+1 åtgärdat) · Fullstack 12 (utveckling i TypeScript – typerna genereras ur schemat) · Cloud 6 (teststrategier och testningens betydelse i CI/CD-pipelines) · Cloud 11 (implementera och integrera automatiserade tester i CI/CD-pipelines)

### Vad jag förstått

**Fullstack 2:** På klientsidan handlar GraphQL-cache om att spara resultat från frågor så att samma fråga med samma variabler kan besvaras utan ett nytt nätverksanrop. Det minskar onödiga requests och gör appen snabbare, men kräver att man förstår vad en fråga faktiskt kostar – både i nätverkstrafik och i serverlast.

**Fullstack 11 och 12:** Ett GraphQL-API kan drabbas av N+1-problemet, där en fråga utlöser många separata databasanrop. Det åtgärdas genom att batcha anropen. Genom att generera TypeScript-typer ur schemat får klienten kompileringstidskontroll, så att ett fält som tas bort i schemat fångas redan vid typecheck.

**Cloud 6 och 11:** Automatiserade tester i en CI/CD-pipeline fångar fel tidigt och gör att varje ändring verifieras likadant innan den driftsätts. En tydlig teststrategi – vad som testas och var – avgör hur mycket pipelinen faktiskt skyddar.

### Var det syns i mitt arbete

**Fullstack 2:** PR #98 – urql-klient med cacheExchange och dokumentcache (`client/src/urql.ts`).
**Fullstack 11 och 12:** PR #99 – genererade typer och dokument med GraphQL Codegen (`client/codegen.ts`, `client/src/gql/`), samt migrering av två vyer till `useQuery`.
