u	2nf that has no transitive dependency with respect to a primary key

- What is *transitive dependency* : if X-> Y then there exist x-> z and z-> y
- 3nf def: a 2nf that has no functional dependency between nonkey attribute
From
![[Pasted image 20260319031506.png|493]]
- ****CAND_NO → CAND_NAME****
- ****CAND_NO → CAND_STATE****
- ****CAND_STATE → CAND_COUNTRY****
- ****CAND_NO → CAND_AGE****

	- ***CAND_NO → CAND_STATE***
	- ***CAND_STATE → CAND_COUNTRY***
	- cand_coun is transitively dependent on cand_no via cand_state
To
![[Pasted image 20260319031444.png|697]]
1. **CANDIDATE (CAND_NO, CAND_NAME, CAND_STATE, CAND_AGE)****
2. ***STATE_COUNTRY (CAND_STATE, CAND_COUNTRY)***