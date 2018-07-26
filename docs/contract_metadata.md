Build Artefact
==============

As compilation succeed Remix create a JSON file for each compiled contract.
These JSON files contains several metadata

Library Deployment
------------------

By default Remix automatically deploy needed libraries.

`linkReferences` contains a map representing libraries which depend on the current contract. 
Values are addresses of libraries used for linking the contract.

`autoDeployLib` defines if the libraries should be auto deployed by Remix or if the contract should be linked with libraries described in `linkReferences`

```
	"VM:-": {
		"linkReferences": {
			"browser/Untitled.sol": {
				"lib": "dddd",
				"lib2": "ess>"
			}
		},
		"autoDeployLib": true
	},
	"main:1": {
		"linkReferences": {
			"browser/Untitled.sol": {
				"lib": "<address>",
				"lib2": "<address>"
			}
		},
		"autoDeployLib": true
	},
	"ropsten:3": {
		"linkReferences": {
			"browser/Untitled.sol": {
				"lib": "<address>",
				"lib2": "<address>"
			}
		},
		"autoDeployLib": true
	},
	...
```
