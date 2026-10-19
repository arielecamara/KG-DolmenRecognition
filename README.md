 KG-DolmenRecognition

Queries Cypher do grafo de conhecimento dos dólmenes de Pavia (Mora) e da paisagem envolvente, da tese de Ariele Câmara (Iscte, 2024; http://hdl.handle.net/10071/35363).

O repositório contém só as queries. Os CSV não estão incluídos. Obtêm-se nas fontes de origem, colocam-se na pasta `import` do Neo4j, e as queries leem-nos com `LOAD CSV` a partir de `file:///`.

O grafo segue o CIDOC-CRM, com CRMgeo, GeoSPARQL e a classe local C1. 

## Ordem

1. `DOLMEN PAVIA (CYPHER) - CSV to KG` — monumentos (`Dolmen2022.csv`).
2. `CAOP - CSV to KG` — limites administrativos, CAOP 2022, DGT (`CAOP2022-Pais.v3.WGS84.csv`).
3. `TipoDeSolo - CSV to KG` — carta de solos, DGADR (`SoilType.UTF8.WGS84.csv`).
4. `COS 1995 (CYPHER) - CSV to KG` a `COS 2018 (CYPHER) - CSV to KG` — uso e ocupação do solo, DGT.
5. `Hidrografia - CSV to KG` — linhas de água (`WaterLine.UTF8.WGS84.csv`).
6. `Curva De Nivel - CSV to KG` — hipsometria (`CountourLine.UTF8.WGS84.csv`).
7. `Queries para arrumar os dados inseridos` — limpeza depois da carga.
8. `Analises Relacionamentos` — proximidade dos dólmenes (Portal do Arqueólogo e Carta Arqueológica) a água, relevo, tipo de solo e uso do solo.
9. `Grid Relations` — grelha espacial e ligações entre camadas.
10. `QUERIES PARA ANALISAR OS DADOS` — consultas de análise, sem CSV.
11. `Queries - KG-ML` — contexto de paisagem de um dólmen para o classificador híbrido. O ficheiro devolve o exemplo com o identificador `D11`.

## Fontes

Uso do solo, hidrografia e CAOP: DGT e APA, pelo SNIG. Carta de solos: DGADR. Hipsometria: Câmara Municipal de Mora, com autorização para o doutoramento. Monumentos: Portal do Arqueólogo e Carta Arqueológica de Mora (2012). Quem tiver acesso a estas fontes reconstrói os CSV e corre as queries.
