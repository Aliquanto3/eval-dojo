# Pistes issues de la veille

Dépôts et articles dont s'inspirer, relevés par la veille sur les agents de code. Ce sont des idées à cadrer, pas des décisions : rien n'a été testé ici. Analyse d'origine : dépôt `veille-agents-code`, `synthese/complement-2026-11-14.md`.

## Vague du 2026-11-14

| Source | Idée à reprendre | Réserve |
|---|---|---|
| [« Agent Evals 101 », Decoding AI](https://www.decodingai.com/p/evaluate-ai-agents-benchmarks-regression-tests) (P. Iusztin, 2026-09-22) | Un plan de leçon sur l'évaluation d'agents. Trois questions : le banc (« ça marche ? », on note le résultat), la non-régression (« ça marche encore ? », on note la trajectoire), l'évaluation en ligne. Trois métriques sur k essais : pass@k (au moins un essai réussit), pass^k (tous réussissent), instabilité = pass@k − pass^k. Règles de montage : vérificateur caché jusqu'à la fin, erreur d'infrastructure jamais comptée comme un échec de l'agent, notes binaires plutôt qu'une échelle de 1 à 5, cas de régression tirés d'échecs réels. | Article de cours adossé à un outil sponsor (Opik). Ses chiffres illustrent, ils ne prouvent rien. |
| [microsoft/PyRIT](https://github.com/microsoft/PyRIT) (MIT) | Un module sur l'évaluation adversariale : reprendre ses familles d'attaque (scans automatiques, attaques sur plusieurs tours) avec un petit modèle servi par Ollama comme cible, pour rester gratuit. | README lu par extraits ; support Windows non vérifié. |
| [Plurai simulation](https://simulation.plurai.ai/connect) | L'idée seulement : décrire les situations qu'un agent peut rencontrer comme un graphe, puis faire jouer des utilisateurs simulés. À présenter comme une famille de méthodes, sans l'outil. | Service hébergé, sans prix, licence ni mesure publiés. |
| [XERJ Query-1](https://xerj.org/blog/xerj-query-ai-model) (article du 2026-11-05, corrigé le 06) | Un exemple de lecture critique : l'article a été corrigé après qu'un lecteur a relevé des métriques manquantes et une comparaison de temps inégale ; les auteurs disent eux-mêmes que le jeu de test vient du jeu de développement et qu'il n'est pas public. Bon support pour apprendre à lire un résultat publié. | — |

Écartés pour ce projet : HKUDS/AgentPilot (mesure des auteurs seulement, dans un cadre d'essais répétés), TechTideOhio/binnacle (v0.0.1).
