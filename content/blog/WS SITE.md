---

description: Initial description.

author: "@Luigi"
---

- Ask sandy about
	- Hugo installation as usuall feature/WS-284
	- Jira board method - Daily standup 4H 15' CET
		- mateo PM
		- TUSHA QA
		- FLOR UX
		- ANDY UX final check
		- allisson DM
		- pc is for sandy as well
	- Qa environments and differences
	- Deploy process
		- ask Dani about how it goes.
- INSTALLATION (I had to go to previous npm versions as with spot on)
	- nvm use 14.15.0
	   npm rebuild node-sass
	   npm install
- MEETING 2022-10-24 (WS Site new stack intro)
	- Are there render.com and builder.io WS accounts?
		- Free ones for builder Rafal will ask andres
		- v1 is netlify + hugo + forestry
		- not forestry in the future
		- alex
			- next.js and builder
	- create private repo
		- use generator next.js
		- minimal site
		- deploy
		- integrate in a builder
		- explore multiple ways of provide content
		- next.js is like rails, serves pages in
			- next.js to provide SSR capabilites
			- generalte content many ways
				- make a request to bulder
				- use builde api to deploy
				- builder provides html or can provide  json of objects.
				- multiples convinations how they 2 provide data.
				- investigate web hooks to
		- How do we mesure performance
			- lighthouse SSR
				-
		- content loaded and hidration (js listeners) make builder look if the document ies uptodate
		- CLOULFLIas cdn
		- section pages data
			-
		- builder.io key (personal) 85a5d1a9ddb04dee9a86780bbbaacc17
	- migrate a single case study first (Beautycounter for instance)
	- before deploying to render.com we have to build a local SSR page with builder.io + next.js
	-
- New site POC with Next.js
	- https://nextjs.org/docs/getting-started
	- ws-site-builder
	- follor steps below
	- https://www.builder.io/c/docs/integrating-builder-pages
-
- What we have achived is deployed is it buildtime? yes!
- 2 other ways
	- for production is how we have done
	- for QA we want the site to fetch newest builder.io version
- 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