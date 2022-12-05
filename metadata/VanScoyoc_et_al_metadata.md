## Definition of column names in *VanScoyoc_et_al_fulldata.csv*

### *Predator-prey dyads & functional traits*

- **pair_ID** -unique ID given to each predator-prey dyad in each study  	
- **reference** -study citation abbreviation and year
- **predator_common** -common name
- **predator_species** -taxanomic species name  	
- **predator_trophic_level** -trophic level in ecological community, best guess as described in paper  	
- **predator_class** - predator guild  	
- **predator_mass_kg** -mass in kilograms (Encyclopedia of Life, Parr et al. 2014)  	
- **predator_mass_category** -binned mass in kilograms   	
- **predator_activity_pattern** -circadian rhythm (Encyclopedia of Life, Parr et al. 2014)  	
- **predator_hunting_mode** -hunting mode (expert advice, Encyclopedia of Life, Parr et al. 2014)  	
- **prey_common** -common name  	
- **prey_species** -taxanomic species name    	
- **prey_trophic_level** -trophic level in ecological community, best guess as described in paper  	
- **prey_order** -taxanomic order name  	
- **prey_mass_kg** -mass in kilograms (Encyclopedia of Life, Parr et al. 2014)	
- **prey_mass_category** - binned mass in kilograms  	
- **prey_activity_pattern** -circadian rhythm (Encyclopedia of Life, Parr et al. 2014)   	


### *Predator-prey temporal overlap data*

- **overlap_low** -overlap coefficient in low human use setting  	
- **CI_low_low** -lower confidence interval of overlap coefficient (low human use setting)  	
- **CI_low_upper** -upper confidence interval of overlap coefficient (low human use setting) 	
- **overlap_high** -overlap coefficient in high human use setting	
- **CI_high_low** -lower confidence interval of overlap coefficient (high human use setting)  	
- **CI_high_upper** -upper confidence interval of overlap coefficient (high human use setting)  	
- **change_overlap** - change in overlap is `overlap_high` - `overlap_low`

### *Predator-prey diel activity data*
*The relevant metric is the `diurnal activity ratio`, taken as the proportion of daytime images for a species at a low/high setting of human use (based on suntime).*

- **pr_D_low_count** -predator, number of daytime images, low human use setting 	
- **pr_N_low_count** -predator, number of nighttime images, low human use setting   	
- **pr_low_total** -predator, total images, low human use setting   		
- **pr_low_D_AR** -predator diurnal activity ratio (`pr_D_low_count` / `pr_low_total`)
- **pr_low_N_AR** -predator nocturnal activity ratio (`pr_N_low_count` / `pr_low_total`)

- **pr_D_high_count** -predator, number of daytime images, high human use setting 	
- **pr_N_high_count** -predator, number of nighttime images, high human use setting   	
- **pr_high_total** -predator, total images, high human use setting   		
- **pr_high_D_AR** -predator diurnal activity ratio (`pr_D_high_count` / `pr_high_total`)
- **pr_high_N_AR** -predator nocturnal activity ratio (`pr_N_high_count` / `pr_high_total`)

- **py_** -all of the same columns are replicated for prey, abbreviated as `py`

### *Behavioral response pathway assignment*

- **hypothesis** -indicates whether the unique predator-prey dyad responses reflected `Mutual Avoidance`, `Mutual Attraction`, `Prey refuge`, or `Predator attraction`  

## Literature Search
Original Web of Science Search (n=4,675) for 2000-2020 (completed on May 13th, 2020)	

Query:
((TS=(("activity pattern*"  OR temporal*  OR diel  OR nocturnal*  OR diurnal*  OR "time of day"  OR "camera trap*"  OR overlap*  OR co-occurrence  OR cooccurrence  OR occupancy)  AND (human*  OR people  OR anthropogenic  OR touris*  OR recreat*  OR disturb*)  AND (wildlife  OR mammal*  OR animal*  OR *carnivor*  OR herbivor*  OR ungulate*  OR predator*  OR prey  OR commun*)NOT(marine*  OR *fish*))  AND SU=((Environmental Sciences & Ecology  OR Zoology  OR Biodiversity & Conservation))))  AND LANGUAGE: (English) AND DOCUMENT TYPES: (Article)	

Refined By:
[excluding]: RESEARCH AREAS: (MARINE FRESHWATER BIOLOGY OR ENGINEERING OR METEOROLOGY ATMOSPHERIC SCIENCES OR LIFE SCIENCES BIOMEDICINE OTHER TOPICS OR WATER RESOURCES OR PUBLIC ENVIRONMENTAL OCCUPATIONAL HEALTH OR TOXICOLOGY OR AGRICULTURE OR URBAN STUDIES OR SCIENCE TECHNOLOGY OTHER TOPICS OR OCEANOGRAPHY OR NEUROSCIENCES NEUROLOGY OR MICROBIOLOGY OR GEOGRAPHY OR REMOTE SENSING OR VETERINARY SCIENCES OR IMAGING SCIENCE PHOTOGRAPHIC TECHNOLOGY OR PUBLIC ADMINISTRATION OR BIOCHEMISTRY MOLECULAR BIOLOGY OR ENTOMOLOGY OR PHYSIOLOGY OR GENETICS HEREDITY OR COMPUTER SCIENCE OR BUSINESS ECONOMICS OR CHEMISTRY OR PHARMACOLOGY PHARMACY OR MATHEMATICS OR PARASITOLOGY OR RADIOLOGY NUCLEAR MEDICINE MEDICAL IMAGING OR BIOPHYSICS OR NUCLEAR SCIENCE TECHNOLOGY OR FISHERIES OR DEVELOPMENTAL BIOLOGY OR ENERGY FUELS OR HISTORY PHILOSOPHY OF SCIENCE OR IMMUNOLOGY OR MATHEMATICAL COMPUTATIONAL BIOLOGY OR PALEONTOLOGY OR REPRODUCTIVE BIOLOGY OR SOCIAL SCIENCES OTHER TOPICS OR ARCHAEOLOGY OR MYCOLOGY OR SOCIOLOGY OR TRANSPORTATION OR ANTHROPOLOGY OR AUDIOLOGY SPEECH LANGUAGE PATHOLOGY OR BIOTECHNOLOGY APPLIED MICROBIOLOGY OR ENDOCRINOLOGY METABOLISM OR ARCHITECTURE OR ART OR DEMOGRAPHY OR DEVELOPMENT STUDIES OR EDUCATION EDUCATIONAL RESEARCH OR FOOD SCIENCE TECHNOLOGY OR GEOCHEMISTRY GEOPHYSICS OR HEALTH CARE SCIENCES SERVICES OR INFECTIOUS DISEASES OR PHILOSOPHY OR TROPICAL MEDICINE OR VIROLOGY) AND [excluding]: WEB OF SCIENCE CATEGORIES: (ORNITHOLOGY OR PSYCHOLOGY OR PSYCHOLOGY MULTIDISCIPLINARY OR PSYCHOLOGY EXPERIMENTAL OR GEOLOGY OR PSYCHOLOGY SOCIAL) AND [excluding]: DOCUMENT TYPES: (PROCEEDINGS PAPER OR BOOK CHAPTER OR DATA PAPER)
	
### Relevant papers were examined further review (n=405)	
To produce the review list of 405 papers, I read abstracts for all studies that had vague titles or were unclear (i.e. “Disturbance maintains alternative biome states” or “On the high trail: examining determinants of site use by the Endangered snow leopard Panthera uncia in Qilianshan, China” or “Occupancy and environmental responses of habitat specialists and generalists depend on dispersal traits”)
	
#### Example reasons for exclusion when reviewing titles/abstracts:	
* **Irrelevant subject** - (e.g. non-mammal, non-empirical, grassland/benthic community, plants, reptiles, insects, birds, public health, computer vision etc.)
* **Irrelevant method**	- surveying local knowledge, walking transects, spoor surveys, using scenting stations, measuring predation clusters, DNA mark-recapture, scat collection, non-empirical review, data collection on one species (i.e. bears with GPS sensors responding to tourism), interview-based occupancy surveys (often used in remote areas, so this could bias included study regions), occupancy from small mammal trapping, flight initiation distance, seasonal counts, mailed surveys, observer teams, acoustic monitoring of birds or anurans, acoustic surveys of a single species (i.e. primate), scenario modelling/predictive modelling
* **Questionable method** - (e.g. arboreal camera trapping, heart rate monitoring), camera traps that failed to detect target species (i.e. 0-10 images), camera surveys with <5 cameras, experiments (e.g. testing chili pepper fence crossing), unsystematic measurement of irrelevant behaviors (e.g. rare image captures, prey carrying behavior, scavenging behavior), baited camera traps
	
#### Example reasons to read full paper:	
* Fits criteria, but not enough information in abstract	multi-mammal occupancy model with no explanation of how data was gathered, studies that reported camera trap surveys alongside other methods (i.e. transects), mammal predator-prey GPS study with activity data of 1hr or less resolution