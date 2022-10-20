# Summary IDA 
## Week 1
- Lecture 1a Intro to DA
- Lecture 1b What is AI
- Lecture 2a Exploratory Data Analysis

### Intro to Data Science and Artificial Intelligence
#### Definition of data, information and knowledge
*Data(some definitions)*
<br>
- Data are just raw facts.
- Data are streams of raw facts representing events before they have been arranged into a form that people can understand and use.
- Data is comprised of facts.
- Recorded symbols.
<br>
Words that keep coming back in different definitions: "raw", "facts", "stream". 
<br>
There is no universal accepted definition of data.
<br>
Data is unprocessed information.
<br>
*Information*
<br>
- Information is commonly thought tho be data, processed or transformed into a form or structure suitable for use by human beings.
- Information is considered a property of data. This implies that the former cannot exist without the ladder.
*Knowledge*
<br>
- Not the same as Information.
- Knowledge is what someone had after understanding information.
- Knowledge is the application/contextualization of information.
- Knowledge is information put into action.
- This is relevant to a decision or area of concern.

*Simple Example*
<br>
outside is 5o C -> it is cold outside -> wear a warm coat.

#### Example
*Given the following situation*
- Movement monitors track a baby's breathing movements and trigger an alarm in vase no movement is detected.
<br>
a. Explain how measurements of baby movements could be transformed from data into information and then into knowledge.
b. Express the knowledge generated at the previous point into a rule which could be implemented.

a). The breating is detected by the sensor (data). If the breathing movement is not present or stops (informaation), then trigger an alarm (knowledge).
b). If no movement then trigger alarm.


### What is Artificial Intelligence
#### Turing test
*What*
<br>
- The turing test is a method wether to determine if a computer is capable of thinking like a human being.
*Problems/Disadvantages*
<br>
- The test can improve chance of passing through psychological strategies.
- Doesn't test the 'intelligence' of the AI, just the responses. (chinese room problem).
- Humans can sometimes be classified as a machine by the Turing test judges.
*Advantages*
<br>
- Objective notion of intelligence.
- Avoids discussion of internal processes and consciousness.
- Eliminates bias in avor of living organism.
*Objections to the Turing test*
<br>
- Bias toward purely symbolic problem solving.
- Constrains machine intelligence to fit human mold.
- It is a disctraction.

#### Views of AI in four catogories
| Thinking humanly | Thinking rationally |
|------------------|---------------------|
|   Acting humanly | Acting rationally   |

<br>
The turing test only test Acting humanly and Acting rationally. These are aswell the most important.
<br>
*Thinking humanly*<br>
- Cognitive revolution: information-processing psychology.
- Requires scientific theories of internal activities of the brain.
- But how do we validate this?
	1. Predicting and testing behavior of human subjects. (top-down/cognitive Science)
	2. Direct identification from neurallogical data. (bottom-up/cognitive neuroscience)
*Thinking rationally*<br>
- What are correct arguments/thought processes?
- The logistic tradition in AI hopes to create intelligent systems using logic programming.
- Problems: 
	- Not all intelligent behavior is mediated by logical deliberation.
	- What is the <ins>purpose of thinking?</ins> What thought should i have out of all the thought that i could have?
*Acting rationally*<br>
- Rational behaviour: doing the right thing.
	- <ins>that which is expected to maximize goal achievement, given the available information.</ins>
*Acting humanly*<br>
- Self explanatory.

#### Examples of what current AI can and cant do
*Go*<br>
- AlphoGo defeats strongest human player in 2016.
- Developed by Google Deepmind.
*Autonomous Driving*<br>
- Driverless robotic car Stanley sped at 22 mph through the Mojave dessert over 132 mile course in 2005.
- Google Self-Driving Car.
*Logistics Planning*<br>
- During the 1991 Gulf War, US forces deployed an AI logistics planning and scheduling program that involved up to 50,000 vehicles, cargo, and people.
*Planning and Scheduling*<br>
- NASA:
	- MAPGEN (2007) plan daily operations for Mars Exploration Rovers.
	- MEXAR2 mission planning for Mars Express Mission (2008).
*Spam Fighting*<br>
- Learning algorithms classify over a billion messages as spam.
*Vacuum cleaning*<br>
- iRobot cooperation has sold 10 million Roomba robotic vacuum cleaners for home use since 2002.

### Exploratory data analysis
#### Complex numbers
Complex numbers consists out of real numbers and imaginary numbers. <br>
- Real numbers for instance: -0, 1, 0.3, pi, e
- Imaginary numbers for instance: i, -i, pi i, ei
- Realnumbers and Imaginary numbers are a subset of complex numbers

take forinstance z as a complex number, then: z = 5 + 3i <br>
5 is a real number, 3i is a imaginary number and (5+3i) is a complex number. <br>
Realnumber part form (z) = 5, also Re(z)=5, Im(z)=3

##### Complex Plane
<img src=imgs/complexplane.png width=25% height=25%>

#### Operations with complex numbers
##### Algebraic addition
- z = a + bi and w = c + di 
- Z + w = a + bi + c + di
- = (a + c) + (b + d)

**Slighty harder example of addition:**<br>
- 2 + 3i + 7i^2 + 5i^3 + 9i^4
- i^2 = -1
- i^3 = i^2 * i = -1 * i = -i
- i^4 = i^2 * i * i = -i^2 = 1
- 2 + (3i) + (7 * -1) + (5 * -i ) + (9 * 1)
- 2 + 3i - 7 - 5i + 9
- 4 - 2i

##### Multiplication
- z * w = (a + bi)(c + di)
- = ac + adi + cbi + bdi^2
- = ac + i(ad + cb) + bdi^2
- = ac + i(ad + cb) + -bd
- = (ac - bd) + i(ad + cb)

##### Division
- z/w = (a + bi/c + di) 
- = (a + bi/c + di) * (c - di/c - di)
- = ((a + bi)(c - di))/((c + di)(c - di))
- = (ac - adi + cdi - bdi^2)/(c^2 - d^2i^2)
- = (ac - i(ad + cd) + bd)/(c^2 - d^2)
- = ((ac + bd)/(c^2 - d^2)) - i((ad + cd)/(c^2 - d^2))


#### Transforming cartesion to polar
- if we have a point on P(3,4) on the cartesian plane we can convert this to the polar plane by using tangus and pythagoras.
- So P(3,4) => P(r,peta):
	- *Calculating r* 
		- r^2 = 3^2 + 4^2
		- r^2 = 9 + 16 
		- r^2 = 25
		- r = sqr(25)
		- r = 5
	- *Calculating peta*
		- tan(peta) = 4/3 (soscastoa/overstaand delen door aanliggend)
		- peta = inverse of tan(4/3)
		- peta = 53.13
	- So P(r,peta) is P(5,53.13)

## Week2
### Agents
#### What is an Agent?
- An <ins>Agent</ins> is an entity that perceives its environment with sensors and acts through the environment actuators.
*Rational Agents: *<br>
- A rational agent srtives to <ins>"do the right thing"</ins> based on what it perceives and what its actions are.
- The right action is the one that will cause the agent to be the most succesful.
	- Performance measure: 
		- is used as an objective criterion for the succes of an agent's behavior.
		- for instance with a vaccuum cleaner:
			- Amount of dirt it cleaned up.
			- cleannes of the environment.
			- Amount of time taken.
			- Amount of electricity consumed.
			- Amount of noise generated.
*Autonomous Agents: *<br>
- An agent is autonomous if its behavior is determined by its own experience.
- With the ability to learn and adapt.
- <ins>A rational agent IS autonomous</ins>.

#### PEAS
- Performance measure
- Environment
- Actuators
- Sensors

*Example for Medical diagnoses agent: *<br>
- Performance measure:
	- Healty patient
	- Minimize costs
	- Lawsuits
- Environment: 
	- Patient
	- Hospital 
	- Staff
- Actuators:
	- Screen display:	
		- Questions	
		- Tests
		- Diagnoses
		- Treatments
		- Referrals
- Sensors:
	- Keyboard
		- Entry of symptoms, symptoms, findings, patient's answers

#### What is an environment
- The nature of an task envionment directly affects the appropiate design for the agent program.
##### Types of environments:
*Fully and Partially Observable environments: *<br>
- A environment is fully observable when the agent's sensor have full acces to the complete state of the environment at each point in time.
- A Partially environment is the opposite ofcours. For instance when sensors don't get the complete state of the environment at each given time due to noise.
*Deterministic and Non Deterministic(stochastic) environments: *<br>
- An environment is deterministic when the next state of the environment is completely determined by the current state of the environment.
- An environment is stochastic when a the next state of the environment is influenced by unpredictable behaviours of the environment.
*Episodic and Sequential environments: *<br>
- An Episodic environment is divided in atomic episodes. In each episode the agent perfoms an action only based on the perception it gets in that episode. previous episodes do not influence the next episode. For instance checking on defective parts on an assembly line. The previous part tells the agent nothing about the next part. 
- In a sequential environment the current decision could affect all the future decisions. Think off chess or or a taxi. 
- Episodic is simpler because it doesnt have to think ahead.
*Static and dynamic environments: *<br>
- An environment is Static when an environment doesnt change while an agent is deliberating.
- In an Dynamic environment the environment can change while the agent is deliberating. 
- Static is simpler because the agent doesnt need to keep track of its environment while deciding its next step.	
*Discrete and Continous environments: *<br>
- An environment is discrete when the agent can perform a limited number of distinct, clearly defined percepts and actions. Such as chess.
- An environment is continous when the agent doesnt have these distinct limited number of actions. For instance a taxi driver, where steering, speed and location of the agent and environment are not distinct limited actions.
*Single-agent and multiple-agent environments: *<br>
- A single-agent environment is an environment in which only one agent acts. For instance a cross-world puzzle.
- A multi-agent environment is an environment in which two or more agents are acting. For instance chess.
- But be carefull with defining an outside influence as an object or agent.

#### Agent architectures
- To increase the generality of agents we have four basic architecture types:
*1.Simple reflex architecture: *<br>
- These agents select actions on the basis of the current percept, ignoring the rest of the percept history.
*2. model-based reflex architecture: * <br>
- These agents behave the same as simple reflex agents but they maintain an internal state.
- This state depends on the percept history and thereby reflects at least some of the unobserved aspects of the current state.
- <ins>Application: </ins> To tackkle partially observable environments. 
*3. Goal-based architecture: *<br>
- Sometimes only knowing the current state is not enough. With a Goal-based architecture the agents needs a goal to know which situations are desirable.
- Typically investigated in serach and planning research.
- Future is taken into account. 
- More flexible since goals are represented explicitly and can be changed.
*4. Utility-based architecture: *<br>
- Sometimes goals can be reached in differ in quality.
- To choose which one is better the utility-based architecture uss an utility function to map states onto a real number.
- Its using its utility tool as a performance measure to improve its goals.


### Pattern Recognition
#### Some problems that suit data mining
- Data mining requires knowledge-based decisions
- There exists a changing environment
- Have sub-optimal current methods
- Not having accesible, sufficient, and relevent data
- Provides high payoff for the right decisions
- Privacy and ethics considerations important if personal data is involved

#### Data mining consists mainly of 6 common tasks:
1. Anomaly detection (outlier/change/deviation detection)
2. Association rule learning (dependency modelling)
3. Clustering (Unsupervised Learning)
4. Classification (Supervised Learning)
5. Regression (Supervised Learning)
6. Summarization

#### Types of learning
*Supervised Learning:*<br>
- Trains a model on known input and output so that it van predict future outputs.
*Unsupervised Learning:*<br>
- Finds hidden patterns or intrinsic structures in data.
*Reinforcement Learning:*<br>
- Rewarding desired behaviours, punishing undesired ones, trial and error.

#### Distance measures
A distance measure should fulfill four conditions:
1. d(P,Q) >= 0
2. d(P,Q) = 0 iff P = Q
3. d(P,Q) = d(Q,P)
4. d(P,Q) =< d(P,W) + d(W,Q) (triangle inequality)
- There are many ways to construct a distance measure

##### Euclidean distance
- P = {p1,p2,...,pn}
- Q = {q1,q2,...,qn}

The Euclidean distance (d) from P to Q
- d(P,Q) = √(q1-p1)^2+(q2-p2)^2+...+(qn-pn)^2
- = √Σ(qi-pi)^2

**Example:**<br>
- 2d plane
- P(5,5) and Q(9,8)
- Geometricaly
<img src="imgs/euclex.png" width=25% height=25%>
- d(P,Q) = √(9-5)^2+(8-5)^2 = √a^2 + b^2 = pietjeachoras

##### Absolute (Manhattan) distance:
<img src="imgs/absdis.png" width=25% height=25%>

##### Infinity distance:
- d(P,Q) = max(|q1 - q2|,....,|qn - pn|)

##### Distance measures based on some property of two points
- Cosine distance = angle between lines from the origin to the points in question.
<img src="imgs/cosdis.png" width=25% height=25%>
- Edit distance = number of inserts and deletes to change TS1 int TS2
- TS1 = {1,2,3,<ins>3</ins>,4,<ins>1</ins>,1} TS2 = {1,2,3,2,4,2,1}

### Mathematical Modelling
	
	
