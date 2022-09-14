

# Introduction to Artificial Intelligence and Data Science
## Lecture 0 5/9/22
### What is data science?
- Data Science is the discipline that describes, predicts and makes casual inferences based on data.

### What is Artificial Intelligence
- Field of science that studies how te create computers or computer software that have intelligent behaviour

### The Data Science Progress
- Data --> Information --> Knowledge

1. <u>Ask</u> an interresting question.
2. <u>Get</u> data.
3. <u>Model</u> data.
4. <u>Communicate</u> and <u>Visualize</u> the Results

#### What is Data?
- Data are <u>facts</u>
- Data can be <u>recorded</u>
- Example: 30 degrees.

#### What is Information?
- Information is data presented in a <u>form/shape</u> that is <u>meaningful</u> to the recipiant.
- Data in <u>context</u>.
- Information can be used because it can be understood.

#### What is Knowledge?
- Looks like information but is absolutely not the same. 
- Knowledge has <u>impact</u> on your <u>decision</u>, information doesn't.
- Knowledge is information ones you put it in <u>action</u>.
- Knowledge are <u>results</u> of <u>understanding</u> information.

##### Excercie/Example
Given the following situation:
- Movement monitors track a baby’s breathing movements and trigger an alarm in case no movement (breathing) is detected.
a. Explain how measurements of baby movements could be transformed from data into information and then into knowledge.
b. Express the knowledge generated at the previous point into a rule which could be implemented

- Answer:
A. First step is to collect the <u>raw breathing data</u> of the baby. The second step is the sensor turning this data in information by detecting if the baby is still breathing. The third step is the human understanding the information and turning it in knowledge by checking upon the baby.
B. IF sensor gives alarm THEN check upon baby.

1. Breathing records = data.
2. The Alarm going of = information.
3. checking upon the baby = knowledge.

ofcours this is viewed from the perspective of a human. 

### Data Scientist Skills
- You must learn to understand your data, look at it critically.
- You are looking for features that will help you determine the best way to handle, process and analyze those data, and enhance the information in the data.
- Prep work is important!

### What to know for/Know how to do for the exam.
- Definition of data, information and knowledge.
- Link between data, information and knowledge.

### Excercise 1
- Given the following situation:
Parking sensors are proximity sensors for road vehicles designed to alert the driver to obstacles while parking.

a. Explain how a measure of proximity between a road vehicle and an obstacle could be transformed from data into information and then into knowledge.
b. Express the knowledge generated at the previous point into a rule which could be implemented into a knowledge based system 

- Answer:
A. First the proximity sensor will collect raw data about the distance between the vehicle and the obstacle. Secondly the the sensor will turn this raw data in information by alarming the user when the vehicle is to close to an obstacle. Lastly the user will turn the information into knowledge by stopping the vehicle on time when the sensor beeps.
B. IF proximity sensor gives alarm THEN Stop vehicle.

### Excercice 2
- Based on the example of Homework 1, try to think of other situations that result in data being 
transferred into information and then knowledge.

- Thermostats are build to measure the room temperature. It can detect certain heights or lows and act upon them by heating or cooling down the airconditioning.

- Answer:
A. First the thermostat will record raw temperatures. Then it will check with the given boundaries by a third party such as a human. If it hits a certain boundaryit will turn this information into knowledge by acting upon these bounderies. It can either heating up or cool down the room.
B. IF Room temperature is to cold THEN start heating room ELSE IF Room temperature too hot THEN start cooling down room.


## Lecture 1 6/9/22 Artificial Intelligence
### Turing test
- A test where a person interacts with a human and AI. 
- The human has to determin if it is interacting with the human or AI.
- If the human cant determin it, it passed the test

#### Problems with the turing test
- Can improve chance of passing through psychological strategies
- Doesn't test 'intelligence', just responses (chinese room problem)
- Humans van 'fail' to convince the judges they are not computers

#### Advantages of turing test
- Objective notion of Intelligence
- Avoids discussion of internal processes and consciousness
- Eliminates bias in favor of living organism

#### Objection to the turing test
- Bias toward purely symbolic problem solving task
- Constrain machine intelligence to fit human mold
- It is a distraction

Altough human-like behaviour can be usefull. For example in the Entertainment industry, Human-Like bot competitors and chatbots given advice.

### More to AI then the turing test
|Thinking Humanly    |Thinking rationally   |
|--------------------|----------------------|
|Acting Humanly      |Acting rationally     |



#### Thinking Humanly 
- Requires scientific theories of internal brain activities
- Need of Cognitive Science and Cognitive Neuroscience

#### Thinking rationally
- Direct line through mathematics and philosophy to modern AI
- Problem: Not all intelligent behaviour is mediated bu logical deliberation


#### Acting rationally
- Rational behaviour: doing the right thing.
- right thing: that which is expected to maximize goal achievement, given the available information
- Doesn't necessarily involve thinking

#### Rational Programs
- Computational limitations make perfect rationality unachievable.
- So we try to create the best program for the given machine resources.

## Lecture 2 8/9/22 
(fourier analysis not needed for exam)
### Data visualization
- The general principle tot display data: <u>as far as possible, to show the original data and try not to obscure the design of the study.</u>
- Show as much data/information as possible.

#### Develop critical/statistical thinking
- Visualization isn't jusst about plotting data. It's about understanding the data and looking at it in a critical way. You are looking for features that will help you determine the mot suitable way to handle, process and analyze those data.
- Think of ww2 airplane example

### Time series data
- sequence of data points, measurements made over a time interval 
- (normally) a quantity over an independent variable (usually time).

#### How dow we identify patterns/structures in a time series?
- Patterns in time series tend to come form <u>repetition</u>.
- Sometimes hard to detect.
- Sometimes you need to change the representation of the time series to detect a pattern.


## Lecture 2 

## Lecture 3 12/9/22 Agents
### What is an agent?
- An agent is anything that can be viewed as <ins>perceiving</ins> through <u>sensors</u> and <u>acting</u> upon that environment through <u>actuators</u>.
- An agent operates autonomoously
- Examples: Humans, robots, softbots, thermostats, etc.

### Abstract form of an agent
- [f: P* -> A]

### Example of agents:
Human agents:
- Sensors: eyes, ears and other organs
- Actuators: hands, legs, mouth and other body parts for actuators

Robotic agents:
- Sensors: Cameras, infrared range finders;
- Actuators: various motors;

### Rational Agents
- A rational agents strives to "do the right thing"
- The right action is the one that makes the agent most succesful
- is autonomous (when an agents behaviour is determined by its own exp)

Formal definition:
- For each possible percept sequence, a rational agent should select an action that is expected to maximise its performance measure, given the evidence procided by the percept sequence and whatever built-in knowledge the agent has.
 
### PEAS
- Performance measure
- Environment
- Actuators
- Sensors

Consider designing an automated taxi:
- Pm: Safe, fast, legal, comf. trp, max. profits.
- E: Roads, other traffic, pedestrians, customers.
- A: Steering wheel, accelorator, brake, signal, horn.
- S: Cameras, sonar, speedometer, GPS, odometer, engine sensors, keyboard.

#### Environment types
##### Fully observable 
- Giving the agent a complete state of the environment at each point in time.
- For instance checkers, you can see the whole board including your own pieces aswell as the oponents pieces.
##### Partially observable
- Giving the agent only a partly state of the environment:
- For instance: poker, You only see your own cards and the cards on the table but not someones other cards.
##### Deterministic
- The next state of the environment is completely determined by the current state and the action executed by the agent.
- For instance Checkers and Stratego.
##### Stochastic
- The next state of the environment is not completely determined by the curren state and the action executed by the agent.
- For instance roulette and boogschieten. 
##### Episodic 
- The Agent's exp is divided into atomic 'episodes' and the choice of actio in each episode depends only on the episode itself.
##### Sequential
- The Agent's exp is divided into atomic 'episodes' and the choice of action can be based on other episodes.
##### Static
- The environment is unchanged while an agent is deliberating.
##### Dynamic
- The environment changes while an agent is deliberating.
##### Discrete
- A limited number of distinct, clearly defined percepts and actions.
##### continuos
- A unlimited number of distinct, clearly defined percepts and actions.
##### Single agent
- An agent operating by itself in an environment
##### Multiagent
- Multiple agents operating in an environment
##### Known 
- State of knowledge of the 'law of physics' of the environment.
##### Unknown
- 

### The Structure of Agents
#### Agent functins and programs
- An agent is specified by the agent function mapping percept sequences to actions
- One agent funcion is rational

##### 4 basic types in order of increasing generality"
1. Simple reflex agents
- Chooses action based only on the current percept.
- Implemented by condition action rules, (if then) rules.
- if dirty then suck
- Only works if the environment is fully observable. otherwise inf loops, think of maze
2. Model-based agents
- To tackle partially observable environments
- Over time update state using world knowledge: How does world change, How do actions affect world.
3. Goal-based agents
- The agents needs a goal to which situations are desirable.
- Typically investigated in search and planning research.
- Future is taken into account.
- Is more flexible since goals are represented explicitly and can be change.
4. Utility-based agents
- Certain goals can be reached in different ways
- Utility function maps a state onto a real number. 
- Improves on goals.

### Exam check list
- Whats an agent?
- When is it rational?
- When is is autonomous?
- PEAS
- Describing environments
- Basic agent architectures


## Lecture 4 13/9/22 Data Mining
### CRISP-DM
- <b>CR</b>oss <b>I</b>ndustry <b>S</b>tandard <b>P</b>rocess for <b>D</b>ata <b>M</b>ining

### Data mining = identifying patterns in data
- Patterns are everywhere: Traffic, Customer service, Human genome, advertisments, etc.

### Problems suitable for data mining
- require knowledge-based decisions
- hae a changing environment
- have sub-optimal current methods
- have accessible, sufficient, and relevent darta
- provideshigh payoff for the right decisions
- privacy and ethics considerations important if personal data is involved.

### Types of learning 
- Supervised learning 
- Unsupervised learning
- Reinforcement learning

### Data mining - tasks
1. Anomaly detection (outlier/change/deviation detection)
2. Association rule learning (dependency modeling)
3. Clustering
4. Classification 
5. Regression 
6. Summarization

- Machine learing: Supervised, Unsupervised or reinforced learning
- Supervised learning: Classification or Regression 
- Unsupervised Learning: Clustering

### Euclidean distance
- insert image, zie note book.




