 
 ## Vecka 40 – TypeScript genom stacken och kvalitetssäkring
**Kursmål:** Fullstack 3 och 12 (TypeScript inom fullstackutveckling: redogöra och genomföra) · Cloud 5 och 6 (metoder och verktyg för kvalitetssäkring · teststrategier och testningens betydelse i pipelinen) · Cloud 13 (argumentera för kvalitetssäkring – ert första beslutsdokument)


### Vad jag förstått
Fullstack 3 och 12: TypeScript är ett måste i modern webbutveckling, det är mycket lättare att fånga visa buggar när man har typkontroll.
Cloud 5 och 6: Vitest funkar lika bra för testing i Vue som i React, det känns väldigt skönt att kunna använda samma verktyg för båda ramverk. Vi använde oss delvis av testpyramid, då vi har flest enhets tester och mindre component tester, vi har inga E2E tester än. Att ha tester i pipelinen unlättar vidare utvecklingen då det fångas visa smaå buggar även innan någon annan reviear kod, det gör det även lättare att lita på sitt egen repo då man vet att den är testat.

### Var det syns i mitt arbete

Cloud 5 och 6: PR #44, skrev enhet och component tester

 
