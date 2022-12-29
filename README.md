# DE_Sprint_final_project

1.	Purpose and description of the project

The project was carried out for the research project "Study and prediction of biodiversity of the superorder Dinosauria".
Final goal of the R&D project: prediction of potential biodiversity of the superorder Dinosauria in each of the geological periods on the territory of Pangea and continents formed after its collapse.

Project objectives:
1.	Creation and patenting of the database created on the basis of paleontological research.
2.	Recording the described species diversity of the superorder Dinosauria for each geological period (each age within a period).
3. Description of a predator-prey model for the superorder Dinosauria with the choice of the Lotka-Voltaire, ArditiHinzburg, and Gauss-Kolmogorov mathematical approach.
4.	Constructing a model of potential species diversity based on paleontological finds across continents.
5.	Construction of a model of potential species diversity on the basis of the selected "predator-prey" model.
6.	Comparison of the obtained models among themselves and with the existing descriptions.
7.	To estimate the "catastrophicity" of the extinction at the Cretaceous-Paleogene boundary.

The objectives of the article were described:
2 - (fixing species diversity by period based on collection of open data in paleobiodb);
3 - using the 10% rule to describe possible predator-prey ratios;
5 - comparing the resulting assumptions with existing descriptions;
7 - concluding that the superorder Dinosauria flourished towards the end of the Cretaceous and a likely "catastrophic" event influenced their extinction.

2.	Data collecting.

We start the project and look at the data to begin with. This step uses only descriptive analytics. The purpose of this step is to understand the weaknesses and strengths of the data used, to determine its sufficiency, and to propose ideas on how to use it. 
During the deployment phase of the project, we received two types of data:
- proprietary - paleodietal data from 1,067 dinosaur species classified into 4 species by type of diet: carnivore, insectivore, omnivore, herbivore. 
- third-party data obtained from two independent paleontological databases: paleobiodb and Dinosauria Genera list.
Based on the data obtained using PostgreSQL, a relational database consisting of three tables was constructed:
The first table includes: id, species name (specie), food type (diet).
The second table includes: id, collection number (colestion_number), latitude coordinate of fossil location (latitude), longitude coordinate of fossil location (longitude), species name (specie).
The third table contains: id, specie, genera, family, type_tishia. 3.

3. Data description
Next, we look at the data available to us.
The description of data in all sources (table, key, number of rows, number of columns).
Using Jupiter NB (Python and the libraries numpy, pandas and matplotlib) we calculated for each column of quantitative data the key statistics on the attributes (minimum, maximum, scatter, deviation, standard deviation, etc.).

4. Data quality.
In this step we record:
1) missing values;
2) data errors (typos);
3) brought the coding of values to a uniform correspondence (for example, the type of movement Ornithischian - bird species, was fixed as the Latin name or as "2", similarly coded types of feeding by numbers and names in different sources were coded types of feeding)

5. Data exploration

Using graphs and tables, explore the data to formulate hypotheses about how the data will help solve the problem.
In a mini-report we record what we found interesting in the data, as well as a list of attributes that are potentially useful.
The data exploration was done in Jupiter NB (using Python and the numpy, pandas, and matplotlib libraries).

Brief conclusions of the study:

1)	Six countries accounted for 75% of all known dinosaur genera; in order, they are the United States, Mongolia, China, Canada, England, and Argentina. Today, the same six countries continue to have the highest known diversities, but in four of the six the number of genera has increased substantially as follows: United States (127 known genera, +48% increase since 1990), China (109, +132%), Argentina (61, +165%), Mongolia (61, +45%), Canada (43, +5%), and England (33, +14%).
2)	In total, we currently recognize 527 valid known genera of dinosaurs (1257 species), excluding genera based on isolated teeth or single elements. All together, 242 new genera have been described since 1990, an 85% increase. 
3)	Diversification shifts are concentrated in the lower (earlier) half of the dinosaur tree Analysis of diversification rates in our dinosaur supertree shows that statistically significant (p < 0.05)
4)	We apply a statistical method, the abundance-based coverage estimator (ACE) (based in Chao model), to account for the incompleteness of the fossil record. We also estimate diversity in the last two stages of the Cretaceous period to address whether dinosaurs were already in decline before their ultimate extinction. Finally, we assess the dependence of known diversity on the availability of fossiliferous rock outcrop, and we predict the trajectory of future dinosaur discoveries. By using the ACE, we currently estimate dinosaur diversity, including genera that remain to be discovered, at 1,844 genera and estimate more than 3500 species.
5)	Usually, when describing the ratio of biological mass of predators and herbivores, the rule of 10 % is resorted to, which says that no more than ten percent of the energy from the previous one is transferred to each successive trophic level. The remaining 90 % is spent on the vital processes of organisms and is dissipated in the form of thermal radiation. Predatory dinosaurs did not necessarily feed only on other dinosaurs. Their diet could include birds, mammals, and other reptiles. However, it is impossible to ignore the predominance of predatory dinosaurs over herbivores in the Jurassic period and the approximate equality between these categories in the Triassic. Even the predominance of herbivores over predators by more than a factor of two in the Cretaceous is insufficient in terms of the generally accepted ecological models. Such a relationship suggests that now we do not know more than one third of the dinosaur species, while their total number may exceed 3500 species.




 


