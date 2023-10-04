# The Software Architect Elevator

by Gregor Hohpe (1st Edition, 2020)

 

---

## Part I

### 1 : Architects

- Architecture and engineering are 2 distinct career paths. Architects tend to have a broader scope, including organizational and strategic aspects, whereas engineers tend to specialize (1)

 

- Architecture is NOT operations. Architects should not ignore productions issues, b/c they provide feedback into potential architectural weaknesses; but architects should not be firefighting.

 

- Architects :

     - job is to <b>make complex topics easy to understand</b>. (2)

     - deal with <i>non-requirements</i> - requirements that aren't explicitly stated, such as : context, tacit assumptions, and hidden dependencies; discovering implicit requirements and making them explicit. (3)

     - "connect the dots" - look at both objects/components and in-between to ensure interdependencies are known/understood (3)

     - see trade-offs - see both pros & cons of decisions/choices and balance tradeoffs inline with overarching goals and principles (3)

     - look <i>beyond</i> products - look beyond product names and feature lists to distill decision options and trade-offs (4)

     - articulate strategy - linking IT and business by translating businessneeds into technical drivers (5)

     - fight complexity - harmonize to reduce complexity (5)

     - by staying grounded in reality and receiving feedback on decisions from real project implementations (5)

     - play a critical role as a connecting and translating element between different layers of an organization (7)

 

- Long project implementation cycles do NOT provide a good <i>learning loop</i> and can lead to an "Architect's Dream, Developer's Nightmare" : architects have achieved their abstact ideals, but the actual implementation is impractical. (9)

 

- Architects who only view from high-level invariably leads to the "<i>authority without responsibility</i>" antipattern - architects must live with, or at least observe, the consequences og their decisions. (9-10)

 

- Disruption is difficult, because <i>systems resist change</i>. (11)

 

### 3 : Architects Live in the First Derivative

- rate of change : a primary factor that influences architecture (22)

 

- the only system that would not benefit from architecture is a static one (on that never changes) (22)

 

- the first derivative : the mathematical expression for how quickly a function's value changes (22)

 

- "living in the first derivative" - good architects deal in/with change and understand the influence change has on architecture (22)

 

- Technology has varying rates of change:

     - low rates of change are more common at the lower levels of the IT stack (hardware, base OS); tend to see more <i>evolution</i> than <i>revolution</i> (23)

     - higher levels tend to move faster, such as (software) frameworks (23)

 

- Software system's First Derivative:

     - think about which part of a software system determines it's rate of change (24) - the build/deployment toolchain (e.g. CICD)

 

- Designing for the First Derivative

     - what aspects <b>IMPEDE</b> change?

          - Dependencies :

               - too many interdependencies between system components will result in small changes neeing adjustments in multple places, increasing both effort AND risk

               - design systems with fewer interdependencies, that they are modular and cleanly seperate responsbibilities (Single Responsibility Principle), and localize changes so that a higher rate of change can be absorbed (25)

               - Accelerate : decoupling system components is the biggest contributor to sustained sotware delivery (25)

          - Friction :

               - ensure software build chain is fully automated by eliminating processes that have long lead times and manual deployment steps (25)

          - Poor Quality :

               - poor quality slows down software delivery (25)

               - testing/changes to a poor quality system take more time and are likely to break things (25)

          - Fear :

               - poor quality and low levels of automation make change risky, this leads to fear of code changes, which leads to stale code (code rot), which in turn increases the risk of changes (25)

    

- Fears slows you down, so confidence speeds you up. Automated tests give teams confidence and thus increase the rate of change. (26)

 

- Without a conscious decision about architecture, the "default" architecture will converge toward the "Big Ball of Mud", akin to a shantytown, in which things are hapharzardly connected/bolted together with no long-term plan/outcome/goal. (26)

 

- Optimizing for local or short-term change can inhibit global or long-term change. (26)

 

- Second Derivative : the rate of change (first derivative) is dependent upon a positive second derivative, that is, <b><i>accelerating</i></b> the rate of change. (28)

     - the essence of transformation (28)

     - for an organization to appreciate and succesfully  conduct a transformative program, it <b>MUST</b> understand economies of speed (28)

 

### 4 : Enterprise Architect or Architect in the Enterprise?

 

- <b>Enterprise architecture</b> (EA) is the organizing logic for business process and IT ingrastructure reflecting the integration and standardization requirements of the company's operating model. (30)

 

- Business arhcitecture describes "the structure of the enterprise in terms of its governance structure, business processes and business information. (31)

 

- Enterprise architecture is the glue between business and IT architecture (32).

 

- IT is a competitive differentiator and opportunity driver, not a commodity like electricity. (33)

 

- EA teams need to have a clearly articulated path to value:any effort that is made needs to be paid back by providing value to the organization. (33)

 

- Due to long feedback cycles inherent in EA plans, which can span multiple years, enterprise architects <i>need to show impact</i>. (33)

 

### 5 : An Architect Stands on Three Legs

 

- a succesful architect must "stand" on 3 legs (38):

     - skill : the foundation for practicing architects, it requires knowledge and the ability to apply it to solve real problems

          - the ability to apply relevant knowledge

          > "Knowledge is like having a drawer chest full of tools. Skill implies knowing when to open which drawer and what tool to use."

     - impact : the measure of how well an architect applies their skill to benefit the company

          - impact is measured by the benefit achieved for the business (39)

     - leadership : determines whether an architect advances the state of the practice

          - mentor juniors architects

          - further the state of a field as whole

 

- Skill without impact is where new architects start as students/apprentices. (39)

 

- Impact without leadership  is the typical place where intermediate architects "plateau" (too ingrained in projects, without expansion). (39)

 

- Leadership without (prior) impact lacks foundation and may be a warning sign of an "ivory tower" architect. (40)

 

- There is a symbiotic relationship between building up skill and applying it. (40)

 

### 6 : Making Decisions

- Being a good architect therefore warrants a conscious effort to becoming a better decision maker. (46)

 

- "the law of small numbers" (bias) : people tend to jump to conclusions based on sample sizes, which can be too small to be statiscally significant. (46)

 

- Prospect Theory (bias) : when faced with an opportunity, people tend to favor smaller but guaranteed gain over the uncertain chance for a larger gain. (48)

 

- Priming : can influence decisions based on recent we data received; can be brought about by setting a context that influences your decision. (48)

 

- Decision trees are very simple methods help us make more rational decisions (50)

 

> "one of an architect's most important tasks is to eliminate irreversibility in software designs" -Martin Fowler

 

- Decisions that can be easily changed later don't need to be made or can be made quickly (52)

 

### 7 : Question Everything

 

- The Five Whys

 

- "why" is a useful question b/c it helps draw attention to the decisions that were made as well as the assumptions and principles that led to those decisions (54)

 

- If you want to change the behavior of the organzation, you often need to identify and overcome outdated assumptions first. (55)

 

- The value of documenting system architectures:

     - faster staff ramp-up

     - reveal architectural inconsistencies

     - allow for rational, fact-based decision making

 

## Part II

 

- three kinds of "architecture" (59):

     1. system architecture, defined by its structure, e.g. microservices architecture

     2. the act of defining a system's rchitectures, e.g. "the architecture committee"

     3. the team that is involved in defining architecture

 

- you choose your architecture OR you let it happen to you (resulting in the "big ball of mud"/shantytown architecture) (60)

 

- "big ball of mud" architecture lacks critical infrastructure and is painful in the longterm (60)

 

- good architecture buys you flexibility (61)

 

- Architects should also strive for conceptual integrity/uniformity across system designs.  Best accomplished by selecting a well-defined set of architecture principles that are consistently appled applied to architectural decisions. Deriving these principles from a declared architecture strategy assures that the decisions support the strategy. (61)

 

- A good architecture is not only consistent across systems but also considers all layers of a software/hardware stack. (61)

 

- https://prodgitlab.usaa.com/grp-cloud-services-private-cicd-tools/terraform/-/merge_requests/312

 

### 8 : Is this Architecture?

 

- a good test for architecture documentation is whether it contains any nontrivial decisions and the rationale behind them. (64)

 

- architecture should NOT dampen creativity, just <i>needless creativity</i>, it also should highligh the importance of making decisions (64)

 

- architectural decision test (65):

     - main components of the system

     - interrelationships between components

     - principles governing it's design (why we did things the way we did)

 

- decisions are driven by system context (66)

 

- documentation highlights relevant decisions and omits unnecessary noise (66)

 

- architectural documentation should illustrate a fairly simple but fundamental decision, documented in an easy-to-understand (67)

 

- architecture is NOT good or bad, it's fit or unfit for purpose (67)

 

- assessing the context and identifying implicit or assumptions in proposed designs is an architect's key responsibility (67)

 

- nonfunctional requirements : hidden assumptions as nonrequirements, requirements that were never explicitly stated (68)

 

- systems architecture does not need to be complicated, but significant decisions need to be well-documented and based on a clear rationale (68)

 

- a good test is whether the chosen option has downsides/tradeoffs - those with none as unlikely to be meaningful (68)

	
