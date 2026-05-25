---
title: "Diagrammes Mermaid"
order: "100"
icon: lucide/chart-pie
---

!!! Note "À propos de Mermaid"
	**Mermaid** est une bibliothèque qui peut être intégrée à n'importe quel projet Javascript, et qui génère des 
	diagrammes à partir de blocs de code Markdown.

	Site web : [mermaid.ai](https://mermaid.ai/open-source/syntax/flowchart.html)


## Flow Chart

=== "📄 Code"

	```md
	````mermaid
	graph LR
	A[Alpha] --> B(Beta) --> C(charlie)
	B --> D(Delta) --> E((Echo))
	A --> F(Foxtrot)
	````
	```

=== "➡️ Résultat"

	```mermaid
	graph LR
	A[Alpha] --> B(Beta) --> C(charlie)
	B --> D(Delta) --> E((Echo))
	A --> F(Foxtrot)
	```


## Pie Chart

=== "📄 Code"

	```md
	````mermaid
	pie title Pets adopted by volunteers
		"Dogs" : 386
		"Cats" : 85
		"Rats" : 15
	````
	```

=== "➡️ Résultat"

	```mermaid
	pie title Pets adopted by volunteers
		"Dogs" : 386
		"Cats" : 85
		"Rats" : 15
	```

## Git 

=== "📄 Code"

	```md
	````mermaid
	%%{init: { 'logLevel': 'debug', 'theme': 'base', 'gitGraph': {'showBranches': false}} }%%
		gitGraph
			commit
			branch hotfix
			checkout hotfix
			commit
			branch develop
			checkout develop
			commit id:"ash" tag:"abc"
			branch featureB
			checkout featureB
			commit type:HIGHLIGHT
			checkout main
			checkout hotfix
			commit type:NORMAL
			checkout develop
			commit type:REVERSE
			checkout featureB
			commit
			checkout main
			merge hotfix
			checkout featureB
			commit
			checkout develop
			branch featureA
			commit
			checkout develop
			merge hotfix
			checkout featureA
			commit
			checkout featureB
			commit
			checkout develop
			merge featureA
			branch release
			checkout release
			commit
			checkout main
			commit
			checkout release
			merge main
			checkout develop
			merge release
	````
	```

=== "➡️ Résultat"

	```mermaid
	%%{init: { 'logLevel': 'debug', 'theme': 'base', 'gitGraph': {'showBranches': false}} }%%
		gitGraph
			commit
			branch hotfix
			checkout hotfix
			commit
			branch develop
			checkout develop
			commit id:"ash" tag:"abc"
			branch featureB
			checkout featureB
			commit type:HIGHLIGHT
			checkout main
			checkout hotfix
			commit type:NORMAL
			checkout develop
			commit type:REVERSE
			checkout featureB
			commit
			checkout main
			merge hotfix
			checkout featureB
			commit
			checkout develop
			branch featureA
			commit
			checkout develop
			merge hotfix
			checkout featureA
			commit
			checkout featureB
			commit
			checkout develop
			merge featureA
			branch release
			checkout release
			commit
			checkout main
			commit
			checkout release
			merge main
			checkout develop
			merge release
	```