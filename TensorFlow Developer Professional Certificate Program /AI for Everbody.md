
@ Puran Z

## Demystifying AI
`AI: ANI, AGI`<br>

ANI: **artificial narrow intelligence** e.g. amart speaker, self-driving car, web search, AI in farming and factories

AGI: **artificial generate intelligence** do anything a human can do

`Machine Learning: software`

Field of study that gives computers the ability to learn without being explicitly programmed.

`Data Science: slide deck`

Science of extracting knowledge and insights from data

`Internet company`

A/B testing<br>
short iteration time<br>
decision making pushed down to engineers and other specialized roles

`AI company`

strategy data acquisition<br>
unified data warehouse<br>
pervasive automation <br>
new roles (e.g. MLE) and division of labor

`AI Transformation`
* excute pilot projects to gain momentum
* build an in-house AI team 
* provide broad AI training
* develop an AI strategy
* develop internal and external communications


## Building AI Projects
`key steps of a machine learning project`
* Collect data
* Train model: iterate many times until good enough
* Deploy model: get data back, maintain/update model

`key steps of a data science project`
* Collect data
* Analyze data: iterate many times to get good insights
* Suggest hypothesis/actions: deploy changes, re-analyze new data periodically

`Brainstorming Framework`
* think about automating tasks rather than automating jobs. e.g., call center routing
* what are the main drivers of business
* what are the main pain points in your business

`You can make progress even without big data`
* having more data almost bever hurt
* data make some business (like web searching) defensible
* but with small datasets, you can still make progress

`Due diligence on project`

**Technical diligence** what AI can do
* can AI system meet desired perfoormance
* how much data is needed
* engineering timeline

**Business diligence** value for your business
* lower costs
* increase revenues
* launch new product or business

`Build vs. buy`
* ML projects can be in-house or outsource
* DS projects are more conmmonly in-house
* Some things will be industry standard - avoid building those

`Specify your acceptance criteria`
* Goal: detect defects with 95% accuracy
* Provide AI team a dataset on which to measure their performance
* Pitfall expecting 100% acc: Limit of ML, insufficient data, mislabeled data, ambiguous labels

`CPU vs. GPU`

CPU: computer processor (Central Process Unit)

GPU: graphics processing unit

`cloud deployment vs. On-premises deployment`


## Building AI in your company

### Case study: smart speaker
`Steps to process the command`
"Hey device, tell me a joke"
* _Trigger word/wakeword detection_: audio -> 'hey device' 0/1
* _Speech recognition_: audio -> 'tell me a joke'
* _Intent recognition_: 'tell me a joke' -> joke? time? music? call? weather?
* _Execute command_

### Case study: Self-drving car
`Steps for deciding how to drive`

Image/Radar/Lidar + GPS, Maps => (Car detection & Pedestrian derection => Trajectory prediction) & Lane detection & Traffic light detection & obstacle detection => Motion Planning => Steer/Accelerate/Brake

### AI Transformation
#### Step1: excute pilot projects to gain momentum
* More important for the initial project to be succeed rather than be the most valuable
* Show traction within 6-12 months
* can be in-house or outsourced

#### Step2: build an in-house AI team 
* AI team supports different BU (Business Unit)
* AI function can be under CTO, CIO, CDO or a new CAIO

#### Step3: provide broad AI training
|Role  	| What they should Learn 	|
|-	|-	|
| Executes and senior business leaders 	|What AI can do for enterprise<br>AI strategy<br>Resource Allocation  	|
| Leaders of divisions working on AI projects 	|  Set project direction(technical and business diligence)<br>Resource allocation<br>Moniter progress 	|
|  AI engineer trainees	| Build and ship AI software<br>Gather data<br>Excute on specific AI project  	|

#### Step4: develop an AI strategy
* Leverage AI to create an adbvantage specific to your industry sector
* Design strategy aligned with the "Virtuous Cycle of AI"<br>
    * -better product-more user- more data-
* Consider creating a data strategy：<br>
    * Strategic data acquisition<br>
    * Unified data warehouse<br>
* Create network effects and platform advantages<br>
    * In industries with "wineer take all" dynamics, AI can be an accelerate

#### Step5: develop internal and external communications
* Investor relations
* Government relations
* Consumer/user education
* Talent/recruitment
* Internal Communications

### AI pitfalls to avoid

## AI and Society
### AI and hype
**the Goldilocks Rule of AI**:<br>
One shoudn't be too optimistic or too pessimistic<br>
### Limitation of AI
* Performance limitations
* explainability is hard(but sometimes doable)

#### Discrimination/Bias
* AI learning unhealthy stereotypes

`Why bias matters`
* hiring tool that discriminated against women
* Facial recognition works better for light-skined than dack-skinned individuals
* bank loan approvals
* Toxic effect of reinforcing unhealthy stereotypes

`Combating bias`
* Technical solutions
    * E.g., "zero out" the bias in words<br>
* Transparenncy or auditing processes
* Diverse workforce

#### Adversarial attacks
* defense do exist, but incur some cost
* similar to spam vs. anti-spam, we may be in arms race for some applications
* physical attack

#### Adverse use of AI
* DeepFakes
    * Synthesize video of people doing things they never did
* Generating fake comments
* Undermining of democracy and privacy
    * Oppressive surveilance
* Spam  vs. anti-spam and fraud vs. anti-fraud


### AI, developing economies
* AI advantage in vertical industry
