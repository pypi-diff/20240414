# Comparing `tmp/multi-agent-decision-0.2.tar.gz` & `tmp/multi-agent-decision-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\multi-agent-decision-0.2.tar", last modified: Sat Mar  4 12:09:47 2023, max compression
+gzip compressed data, was "multi-agent-decision-0.3.tar", last modified: Sun Apr 14 03:58:10 2024, max compression
```

## Comparing `multi-agent-decision-0.2.tar` & `multi-agent-decision-0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-04 12:09:47.000000 multi-agent-decision-0.2/
--rw-rw-rw-   0        0        0    20279 2023-03-04 12:09:47.000000 multi-agent-decision-0.2/PKG-INFO
--rw-rw-rw-   0        0        0    17846 2023-03-04 09:26:14.000000 multi-agent-decision-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-04 12:09:47.000000 multi-agent-decision-0.2/multi_agent_decision/
--rw-rw-rw-   0        0        0      153 2023-03-04 10:19:14.000000 multi-agent-decision-0.2/multi_agent_decision/__init__.py
--rw-rw-rw-   0        0        0    33238 2023-03-04 12:04:04.000000 multi-agent-decision-0.2/multi_agent_decision/simulation.py
-drwxrwxrwx   0        0        0        0 2023-03-04 12:09:47.000000 multi-agent-decision-0.2/multi_agent_decision.egg-info/
--rw-rw-rw-   0        0        0    20279 2023-03-04 12:09:47.000000 multi-agent-decision-0.2/multi_agent_decision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-03-04 12:09:47.000000 multi-agent-decision-0.2/multi_agent_decision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-04 12:09:47.000000 multi-agent-decision-0.2/multi_agent_decision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-03-04 12:09:47.000000 multi-agent-decision-0.2/multi_agent_decision.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-03-04 12:09:47.000000 multi-agent-decision-0.2/multi_agent_decision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-03-04 12:09:47.000000 multi-agent-decision-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1419 2023-03-04 12:08:32.000000 multi-agent-decision-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:58:10.280988 multi-agent-decision-0.3/
+-rw-rw-rw-   0        0        0     1089 2022-04-10 15:29:14.000000 multi-agent-decision-0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0    18907 2024-04-14 03:58:10.280988 multi-agent-decision-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    17846 2023-03-04 09:26:14.000000 multi-agent-decision-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 03:58:10.280988 multi-agent-decision-0.3/multi_agent_decision/
+-rw-rw-rw-   0        0        0      153 2023-03-04 10:19:14.000000 multi-agent-decision-0.3/multi_agent_decision/__init__.py
+-rw-rw-rw-   0        0        0    34486 2024-04-14 03:54:06.000000 multi-agent-decision-0.3/multi_agent_decision/simulation.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:58:10.280988 multi-agent-decision-0.3/multi_agent_decision.egg-info/
+-rw-rw-rw-   0        0        0    18907 2024-04-14 03:58:09.000000 multi-agent-decision-0.3/multi_agent_decision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2024-04-14 03:58:09.000000 multi-agent-decision-0.3/multi_agent_decision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 03:58:09.000000 multi-agent-decision-0.3/multi_agent_decision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2024-04-14 03:58:09.000000 multi-agent-decision-0.3/multi_agent_decision.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-14 03:58:09.000000 multi-agent-decision-0.3/multi_agent_decision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2024-04-14 03:58:10.296611 multi-agent-decision-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1455 2024-04-14 03:49:19.000000 multi-agent-decision-0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `multi-agent-decision-0.2/PKG-INFO` & `multi-agent-decision-0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,189 +1,189 @@
 Metadata-Version: 2.1
 Name: multi-agent-decision
-Version: 0.2
+Version: 0.3
 Summary: Simulates the actions which agents take under multi-agent systems and social networks
 Home-page: https://github.com/ankur-tutlani/multi-agent-decision
+Download-URL: https://github.com/ankur-tutlani/multi_agent_decision/archive/refs/tags/v_03.tar.gz
 Author: ankurtutlani
 Author-email: ankur.tutlani@gmail.com
 License: MIT
-Download-URL: https://github.com/ankur-tutlani/multi_agent_decision/archive/refs/tags/v_02.tar.gz
-Description: 
-        # Decision-making under Multi-Agent Systems and Social Networks
-        
-        This library is used to ascertain how agents take decisions under multi-agent systems. Agents are connected with other agents via a social network and play symmetric games. Agents take decisions based upon their interactions with other agents in the neighbourhood. The strategy which is being played most frequently by agents and for a longer duration of time is a potential candidate for being called a norm. This library demonstrates how norms evolve from bottom-up when agents interact with other agents and decide what is best for them.
-        
-        
-        ## How to use it?
-        
-        
-        ```bash
-          # Install
-          pip install multi-agent-decision
-        
-          
-          # Import
-          from multi_agent_decision import simulation
-        
-          # Execute 
-          simulation.simulation_function_neighbors(random_seed = 226822,
-                                         iteration_name = "test1",
-                                         path_to_save_output = "C:\\Users\\Downloads\\",
-                                         num_strategies=3,
-                                         agent_initial_state =[],
-                                         strategy_share = [0.4,0.4,0.2],
-                                         strategy_pair = {0: "H",1: "M",2: "L"},
-                                         payoff_values = [[0,0,70],[0,50,50],[30,30,30]],
-                                         network_name = "small_world1",
-                                         prob_edge_rewire = 0.50,
-                                         grid_network_m = 5,
-                                         grid_network_n = 8,
-                                         num_agents = 20, 
-                                         num_neighbors = 2,
-                                         delta_to_add = 20,
-                                         norms_agents_frequency = 0.7,
-                                         norms_time_frequency = 0.5,
-                                         min_time_period = 20,
-                                         enable_delta_payoff = "Yes",
-                                         num_of_trials = 50,
-                                         fixed_agents = [5,9],
-                                         fixed_strategy_to_use = 0,
-                                         function_to_use = "perturbed_response4",
-                                         perturb_ratio = 0.05
-                                          
-                                         )
-        
-        
-        ```
-            
-        ## Function parameters
-        Following are the parameters which are required to be specified. At the end in the parenthesis, it shows the data type of the parameter which is required or the possible values which is required to be used. In following we will use agents' strategies, actions, choices, responses interchangeably. These all represent same intent and meaning in our context.  
-        
-        1. random_seed : Random seed to reproduce results. (Integer)
-        2. iteration_name: Give any name for this iteration. (String)
-        3. path_to_save_output : The location where output excel files should be saved. (String)
-        4. num_strategies : Total number of strategies. (Integer)
-        5. agent_initial_state : Specify the initial state of agents in list format e.g. ["H","M","M"] in case of 3 agents where 1st agent follows "H" strategy and agents 2 and 3 follow "M". (List)
-        6. strategy_share : Percent distribution of strategies among agents. Must be specified in list format. E.g.[0.4,0.4,0.2]. Must add up to 1. Specify in the order of strategies 0,1,2, and so on. (List)
-        7. strategy_pair : Strategy pair in dictionary format. E.g. {0: "H",1: "M",2: "L"}. 0 strategy is "H", 1 strategy is "M", and so on. Count must match with num_strategies argument. Keys would need to be 0,1,2, etc. Value corresponding to keys can be anything in string format. (Dict)
-        8. payoff_values : List of payoff values. E.g. [[0,0,70],[0,50,50],[30,30,30]]. The first list [0,0,70] is the first row of the 3*3 payoff matrix assuming we have 3 strategies. Second list [0,50,50] is the second row of the payoff matrix and third list [30,30,30] is the third row of payoff matrix.(List)
-        9. network_name : Specify one of these values. A detailed explanation is provided below. ["small_world1","small_world2","small_world3","complete","random","grid2d"]. (String)
-        10. prob_edge_rewire : Small world network parameter. Probability of rewiring existing edges or adding new edges. (Float)
-        11. grid_network_m :  2-dimensional grid network parameter. Number of nodes. (Integer)
-        12. grid_network_n :  2-dimensional grid network parameter. Number of nodes. (Integer)
-        13. num_agents : Number of agents. (Integer)
-        14. num_neighbors : Number of neighbours. (Integer)
-        15. delta_to_add : Delta payoff value which will be added (or deducted in case of negative value) to the payoffs in case of norm displacement. (Float/Integer)
-        16. norms_agents_frequency : Norm condition. Minimum percentage of agents required to use same strategy. Specify number from 0 (0% agents) to 1(100% agents). (Float)
-        17. norms_time_frequency : Norm condition. Minimum percentage of times agents require to use same strategy. Specify number from 0 (no time period) to 1 (all time periods). (Float)
-        18. min_time_period : Minimum time period for which the game should be run before adding delta payoff. (Integer)
-        19. enable_delta_payoff : If norm displacement is required to be assessed , specify "Yes" else specify "No".
-        20. num_of_trials : Number of trials, how long game should run. (Integer)
-        21. fixed_agents : Agents assumed as fixed. e.g. [2,3] shows we want agents 2 and 3 to be fixed. (List)
-        22. fixed_strategy_to_use : Specify key value from strategy_pair. e.g. if we want fixed agents to follow strategy "H" and strategy_pair is {0: "H",1: "M",2: "L"}, specify the value as 0. (Integer)
-        23. function_to_use : Specify one of these values. A detailed explanation is provided below. ["perturbed_response1","perturbed_response2","perturbed_response3","perturbed_response4"]. (String)
-        24. perturb_ratio : Probability of agents taking action randomly. (Float)
-        
-        
-        <br />
-        
-        In the "function_to_use" parameter above, below is the explanation for what these different values mean inside the list specified above.
-        
-        1. perturbed_response1: Agents select the best response (1-perturb_ratio)*100% times among the strategies which are most frequently used. If there is more than one such strategy, then agents select any one strategy randomly. Agents select random strategy (perturb_ratio)*100% times among the strategies which are not most frequently used. Here also, if there is more than one such strategy, then agents select any one strategy randomly out of these.
-        2. perturbed_response2: Agent selects strategy randomly according to the relative weightage of different strategies. These relative weights are the % of times the respective strategy has been used by opponents in the past. 
-        3. perturbed_response3: This is same as "perturbed_response1" function except agent selects random strategy (perturb_ratio)*100% times from all the possible strategies and not only from the ones which were not used most frequently by their opponents.
-        4. perturbed_response4: Agent selects the best response 100% of times among the strategies which are most frequently used. If there is more than one such strategy, then agents select any one strategy randomly. There is no perturbation element (perturb_ratio is considered as zero).
-        
-        
-        <br/>
-        
-        In the "network_name" parameter above, below is the explanation for what these different values mean inside the list specified above.
-        1. small_world1: Returns a Watts Strogatz small-world graph. Here number of edges remained constant once we increase the prob_edge_rewire value. Shortcut edges if added would replace the existing ones. But total count of edges remained constant.
-        2. small_world2: Returns a Newman Watts Strogatz small-world graph. Here number of edges increased once we increase the prob_edge_rewire value. It would add more shortcut edges in addition to what already exist.
-        3. small_world3: Returns a connected Watts Strogatz small-world graph. Rest of the explanation remains as small_world1.
-        4. complete: Returns the complete graph.
-        5. random: Compute a random graph by swapping edges of a given graph. The given graph used is Watts Strogatz small-world graph (the one produced by "small_world1").
-        6. grid2d: Return the 2d grid graph of mxn nodes, each connected to its nearest neighbors.
-        
-        We have used the networkx python library to populate these graphs. For more information around these graphs and how these are produced please refer to the link in the reference section.
-        
-        
-        
-        ## Function explanation
-        Here we explain the underlying functioning of this library with the help of an example. But this can be replicated to any symmetric game wherein we have defined finite strategies along with its payoff values.
-        
-        We assume there is a Nash demand game wherein each agent can make 3 demands, High (70), Medium (50) or Low (30). The rule of the game is if the total demands made by two agents in any given iteration are more than 100, no one is going to get anything. Below is the payoff matrix of row versus column player looks like.
-        
-        		  H	  M	    L
-            H	(0,0)	(0,0)	 (70,30)
-            M	(0,0)	(50,50)	 (50,30)
-            L	(30,70)	(30,50)	 (30,30)
-        	
-        
-        There are 3 pure strategy Nash equilibria, (H, L), (M, M) and (L, H). There is not a strictly or weakly dominant strategy for any of the row or column player. Suppose that agents are connected in a ring network wherein each agent is connected with two other agents, one on the left and one on the right like in below image.
-        
-        
-        ![](https://github.com/ankur-tutlani/multi-agent-decision/raw/main/network_graph.png)
-        
-        
-        Agents update their strategy if any of their neighbours (defined by "num_neighbors") are having higher payoff else, they stick to their own strategy which they have been following. Payoffs are computed as follows. If agent with strategy H meets agent with strategy M and L, then payoff from meeting with strategy M agent equals 0 and payoff from meeting with strategy L agent equals 70, hence the total payoff equals 70. In case of a tie, meaning payoffs are exactly same following current strategy versus payoffs from neighbours" strategy then agents stick to the strategy which they have been following. 
-        
-        We assume agents are distributed in a specific ratio in a network. E.g., if total agents ("num_agents") are 20 and if they are distributed in 40/40/20 distribution ("strategy_share"), that implies there are 8 H type agents, 8 M type agents and 4 L type agents. This can be represented in a list format like this [H,H,H,H,H,H,H,H,M,M,M,M,M,M,M,M,L,L,L,L]. This list shows first agent follows "H" (first value from the left), last agent follows "L" (last value from the right), agent 16 follows "M" etc.This list can be rearranged in multiple ways but still satisfies the condition of 40/40/20. Hence, we require to specify initial state of the agents in "agent_initial_state" parameter in the list format. If this parameter is empty, the function will select any one state randomly. This initial state is being shown in "initial_state_considered_..."  excel file output. For more details on the output generated, please refer to the section below.
-        
-        We start the game with one edge of the network is selected at any given point. Edge of the network is represented as (0,1), (5,4) etc, implying agents 0 and 1 are connected with each other, agents 5 and 4 are connected with each other. During each time period, all edges are selected sequentially and the agents associated with those edges play the game. We are interested in knowing how the initial state of H/M/L distribution changes as agents interact over a period of time and update their strategy. And how these results change when agents start the game with different initial states (e.g. more H type agents placed with H types or more H type agents placed with M type etc.).
-        
-        We have considered different combinations of strategies that agents can adopt while taking actions. We assume that agents use perturbed best response implying agents can take action randomly out of H,M or L with a certain positive probability (Young, 2015). At each time when agents require to take action, they look at the strategies of their neighbours and calculate their payoff. All agents calculate their payoffs in the current period and decide if they want to change strategies or stick to what they have been following so far. We have tested four different ways which agents can use to decide what action to take. The "function_to_use" parameter provides details about these and how these are different to each other.
-        
-        When the simulations are run for "num_of_trials" timeperiod, we get the percentage distribution of  H/M/L which agents used. This shows the percentage of agents who used H/M or L during each time period. The strategy which satisfy the two conditions for norm specified by "norms_agents_frequency" and "norms_time_frequency" are considered as norm. We have looked at two dimensions of norms, number of agents following the norm and for how long it has been followed. We can see the output like below. In below graph, X-axis shows the timeperiod, and Y-axis shows the % of agents who played the respective strategy. Y-axis values are in ratio format (range from 0 - 1), so would need to multiply by 100 to get this in percentage format. 
-        
-        
-        ![](https://github.com/ankur-tutlani/multi-agent-decision/raw/main/norm_emergence.png)
-        
-        
-        
-        In above figure, strategy "M" satisfies the norm criteria, when we assume "norms_agents_frequency" as 0.7 and "norms_time_frequency" as 0.5. This implies at least 70% of agents following "M" for at least 50% of times. The detailed explanation of the output generated is provided in the next section.
-        
-        We have also considered the possibility of norm displacement. This is controlled by three parameters, "enable_delta_payoff", "delta_to_add", and "min_time_period" parameters. For norm displacement, we need to specify "enable_delta_payoff" value to "Yes" and also specify a positive/negative value for "delta_to_add" parameter. The "min_time_period" parameter specifies the minimum time period for which the game should run before checking for norm displacement. Its value should be set lower than "num_of_trials" parameter. When any strategy satisfies the norm criteria laid out (say "M"), then the "delta_to_add" value is being added to the payoff values for rest of the other strategies ("H" and "L") after "min_time_period". The revised payoff matrix would be used by agents once the delta value is added to the payoff values. This would continue as long as some other strategy satisfies the norm criteria and the game is still not played for "num_of_trials" timeperiods. If some other strategy now satisfies the norm criteria (say "H"), then the delta payoff value would be added to the rest of the strategies ("M" and "L"). And this process continues till the game is played for all the timeperiods ("num_of_trials"). This can be seen in below figure where "M" strategy is being displaced by "H" strategy after around 40 timeperiods. And then again there is an attempt to displace "H" strategy with "M" strategy later in the game at around 90th timeperiod.
-        
-        
-        ![](https://github.com/ankur-tutlani/multi-agent-decision/raw/main/norm_displacement.png)
-        
-        
-        
-        ## How to interpret output?
-        There are total 10 files generated in the output when there is at least 1 strategy which satisfies the norm criteria.
-        
-            input_network_ringnetwork_2023-02-02-21-31-34.png
-            networkgraph_initial_state_ringnetwork_2023-02-02-21-31-34.png
-            strategy_trend_ringnetwork_2023-02-02-21-31-34.png
-        	network_after_100_timeperiods_ringnetwork_2023-02-02-21-31-34.png
-            normcandidates_ringnetwork_2023-02-02-21-31-34.xlsx
-            time_when_reached_norm_ringnetwork_2023-02-02-21-31-34.xlsx
-        	parameters_ringnetwork_2023-02-02-21-31-34.xlsx
-        	aggregate_data_detailed_agent_ringnetwork_2023-02-02-21-31-34.xlsx
-            initial_state_considered_ringnetwork_2023-02-02-21-31-34.xlsx
-        	payoff_matrices_considered_by_timeperiod_ringnetwork_2023-02-02-21-31-34.xlsx
-            
-        
-        
-        The 4 image files (.png) contain the network graphs and trend graph which is being considered for the simulation. The "input_network_.." file is the input network with which the game is started. "networkgraph_initial_state_...." file shows initial strategy distribution in the ratio specified in "strategy_share" parameter. The "strategy_trend_..." file shows the percent of agents following "H","M" or "L" strategy at each time period during the game. The "network_after_..." file is the network state at the end of game. Agents following the same strategy would be coloured in the same colour in this file.
-        
-        Norm file "normcandidates_..." shows strategy that satisfies the norm criteria laid out. File "time_when_reached_norm_..." shows the time period number when the specific strategy met the norm criteria. These 2 files are generated only when at least one strategy satisfies the norm criteria. 
-        
-        Parameters file "parameters_.." lists all the parameters which have been specified in the function call. File "aggregate_data_detailed_.." has the information on percentage of agents who proposed different strategies at each time period during the game. "initial_state_considered_" file shows the initial state with which game is started. In case of norm displacement, "payoff_matrices_considered_.." shows the payoff matrix considered along with time period. When there is more than one row in this file, this shows payoff matrix is being revised during the simulation run. The timeperiod column in this file shows the time period point at which the payoff matrix is revised.
-        
-        All the file names end with date and time stamp when the function was executed. It also contains information on network structure used like "ringnetwork" or "smallworld" network etc.
-        
-        
-        ## References
-        1. Young, H.P. "The evolution of social norms" Annual Review of Economics. 2015 (7),pp.359-387
-        2. https://pypi.org/project/networkx/ 
-        
-        
 Keywords: game theory,evolutionary game,social norms,multi-agent systems,evolution,social network,computational economics,simulation,agent-based modeling,computation
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+
+# Decision-making under Multi-Agent Systems and Social Networks
+
+This library is used to ascertain how agents take decisions under multi-agent systems. Agents are connected with other agents via a social network and play symmetric games. Agents take decisions based upon their interactions with other agents in the neighbourhood. The strategy which is being played most frequently by agents and for a longer duration of time is a potential candidate for being called a norm. This library demonstrates how norms evolve from bottom-up when agents interact with other agents and decide what is best for them.
+
+
+## How to use it?
+
+
+```bash
+  # Install
+  pip install multi-agent-decision
+
+  
+  # Import
+  from multi_agent_decision import simulation
+
+  # Execute 
+  simulation.simulation_function_neighbors(random_seed = 226822,
+                                 iteration_name = "test1",
+                                 path_to_save_output = "C:\\Users\\Downloads\\",
+                                 num_strategies=3,
+                                 agent_initial_state =[],
+                                 strategy_share = [0.4,0.4,0.2],
+                                 strategy_pair = {0: "H",1: "M",2: "L"},
+                                 payoff_values = [[0,0,70],[0,50,50],[30,30,30]],
+                                 network_name = "small_world1",
+                                 prob_edge_rewire = 0.50,
+                                 grid_network_m = 5,
+                                 grid_network_n = 8,
+                                 num_agents = 20, 
+                                 num_neighbors = 2,
+                                 delta_to_add = 20,
+                                 norms_agents_frequency = 0.7,
+                                 norms_time_frequency = 0.5,
+                                 min_time_period = 20,
+                                 enable_delta_payoff = "Yes",
+                                 num_of_trials = 50,
+                                 fixed_agents = [5,9],
+                                 fixed_strategy_to_use = 0,
+                                 function_to_use = "perturbed_response4",
+                                 perturb_ratio = 0.05
+                                  
+                                 )
+
+
+```
+    
+## Function parameters
+Following are the parameters which are required to be specified. At the end in the parenthesis, it shows the data type of the parameter which is required or the possible values which is required to be used. In following we will use agents' strategies, actions, choices, responses interchangeably. These all represent same intent and meaning in our context.  
+
+1. random_seed : Random seed to reproduce results. (Integer)
+2. iteration_name: Give any name for this iteration. (String)
+3. path_to_save_output : The location where output excel files should be saved. (String)
+4. num_strategies : Total number of strategies. (Integer)
+5. agent_initial_state : Specify the initial state of agents in list format e.g. ["H","M","M"] in case of 3 agents where 1st agent follows "H" strategy and agents 2 and 3 follow "M". (List)
+6. strategy_share : Percent distribution of strategies among agents. Must be specified in list format. E.g.[0.4,0.4,0.2]. Must add up to 1. Specify in the order of strategies 0,1,2, and so on. (List)
+7. strategy_pair : Strategy pair in dictionary format. E.g. {0: "H",1: "M",2: "L"}. 0 strategy is "H", 1 strategy is "M", and so on. Count must match with num_strategies argument. Keys would need to be 0,1,2, etc. Value corresponding to keys can be anything in string format. (Dict)
+8. payoff_values : List of payoff values. E.g. [[0,0,70],[0,50,50],[30,30,30]]. The first list [0,0,70] is the first row of the 3*3 payoff matrix assuming we have 3 strategies. Second list [0,50,50] is the second row of the payoff matrix and third list [30,30,30] is the third row of payoff matrix.(List)
+9. network_name : Specify one of these values. A detailed explanation is provided below. ["small_world1","small_world2","small_world3","complete","random","grid2d"]. (String)
+10. prob_edge_rewire : Small world network parameter. Probability of rewiring existing edges or adding new edges. (Float)
+11. grid_network_m :  2-dimensional grid network parameter. Number of nodes. (Integer)
+12. grid_network_n :  2-dimensional grid network parameter. Number of nodes. (Integer)
+13. num_agents : Number of agents. (Integer)
+14. num_neighbors : Number of neighbours. (Integer)
+15. delta_to_add : Delta payoff value which will be added (or deducted in case of negative value) to the payoffs in case of norm displacement. (Float/Integer)
+16. norms_agents_frequency : Norm condition. Minimum percentage of agents required to use same strategy. Specify number from 0 (0% agents) to 1(100% agents). (Float)
+17. norms_time_frequency : Norm condition. Minimum percentage of times agents require to use same strategy. Specify number from 0 (no time period) to 1 (all time periods). (Float)
+18. min_time_period : Minimum time period for which the game should be run before adding delta payoff. (Integer)
+19. enable_delta_payoff : If norm displacement is required to be assessed , specify "Yes" else specify "No".
+20. num_of_trials : Number of trials, how long game should run. (Integer)
+21. fixed_agents : Agents assumed as fixed. e.g. [2,3] shows we want agents 2 and 3 to be fixed. (List)
+22. fixed_strategy_to_use : Specify key value from strategy_pair. e.g. if we want fixed agents to follow strategy "H" and strategy_pair is {0: "H",1: "M",2: "L"}, specify the value as 0. (Integer)
+23. function_to_use : Specify one of these values. A detailed explanation is provided below. ["perturbed_response1","perturbed_response2","perturbed_response3","perturbed_response4"]. (String)
+24. perturb_ratio : Probability of agents taking action randomly. (Float)
+
+
+<br />
+
+In the "function_to_use" parameter above, below is the explanation for what these different values mean inside the list specified above.
+
+1. perturbed_response1: Agents select the best response (1-perturb_ratio)*100% times among the strategies which are most frequently used. If there is more than one such strategy, then agents select any one strategy randomly. Agents select random strategy (perturb_ratio)*100% times among the strategies which are not most frequently used. Here also, if there is more than one such strategy, then agents select any one strategy randomly out of these.
+2. perturbed_response2: Agent selects strategy randomly according to the relative weightage of different strategies. These relative weights are the % of times the respective strategy has been used by opponents in the past. 
+3. perturbed_response3: This is same as "perturbed_response1" function except agent selects random strategy (perturb_ratio)*100% times from all the possible strategies and not only from the ones which were not used most frequently by their opponents.
+4. perturbed_response4: Agent selects the best response 100% of times among the strategies which are most frequently used. If there is more than one such strategy, then agents select any one strategy randomly. There is no perturbation element (perturb_ratio is considered as zero).
+
+
+<br/>
+
+In the "network_name" parameter above, below is the explanation for what these different values mean inside the list specified above.
+1. small_world1: Returns a Watts Strogatz small-world graph. Here number of edges remained constant once we increase the prob_edge_rewire value. Shortcut edges if added would replace the existing ones. But total count of edges remained constant.
+2. small_world2: Returns a Newman Watts Strogatz small-world graph. Here number of edges increased once we increase the prob_edge_rewire value. It would add more shortcut edges in addition to what already exist.
+3. small_world3: Returns a connected Watts Strogatz small-world graph. Rest of the explanation remains as small_world1.
+4. complete: Returns the complete graph.
+5. random: Compute a random graph by swapping edges of a given graph. The given graph used is Watts Strogatz small-world graph (the one produced by "small_world1").
+6. grid2d: Return the 2d grid graph of mxn nodes, each connected to its nearest neighbors.
+
+We have used the networkx python library to populate these graphs. For more information around these graphs and how these are produced please refer to the link in the reference section.
+
+
+
+## Function explanation
+Here we explain the underlying functioning of this library with the help of an example. But this can be replicated to any symmetric game wherein we have defined finite strategies along with its payoff values.
+
+We assume there is a Nash demand game wherein each agent can make 3 demands, High (70), Medium (50) or Low (30). The rule of the game is if the total demands made by two agents in any given iteration are more than 100, no one is going to get anything. Below is the payoff matrix of row versus column player looks like.
+
+		  H	  M	    L
+    H	(0,0)	(0,0)	 (70,30)
+    M	(0,0)	(50,50)	 (50,30)
+    L	(30,70)	(30,50)	 (30,30)
+	
+
+There are 3 pure strategy Nash equilibria, (H, L), (M, M) and (L, H). There is not a strictly or weakly dominant strategy for any of the row or column player. Suppose that agents are connected in a ring network wherein each agent is connected with two other agents, one on the left and one on the right like in below image.
+
+
+![](https://github.com/ankur-tutlani/multi-agent-decision/raw/main/network_graph.png)
+
+
+Agents update their strategy if any of their neighbours (defined by "num_neighbors") are having higher payoff else, they stick to their own strategy which they have been following. Payoffs are computed as follows. If agent with strategy H meets agent with strategy M and L, then payoff from meeting with strategy M agent equals 0 and payoff from meeting with strategy L agent equals 70, hence the total payoff equals 70. In case of a tie, meaning payoffs are exactly same following current strategy versus payoffs from neighbours" strategy then agents stick to the strategy which they have been following. 
+
+We assume agents are distributed in a specific ratio in a network. E.g., if total agents ("num_agents") are 20 and if they are distributed in 40/40/20 distribution ("strategy_share"), that implies there are 8 H type agents, 8 M type agents and 4 L type agents. This can be represented in a list format like this [H,H,H,H,H,H,H,H,M,M,M,M,M,M,M,M,L,L,L,L]. This list shows first agent follows "H" (first value from the left), last agent follows "L" (last value from the right), agent 16 follows "M" etc.This list can be rearranged in multiple ways but still satisfies the condition of 40/40/20. Hence, we require to specify initial state of the agents in "agent_initial_state" parameter in the list format. If this parameter is empty, the function will select any one state randomly. This initial state is being shown in "initial_state_considered_..."  excel file output. For more details on the output generated, please refer to the section below.
+
+We start the game with one edge of the network is selected at any given point. Edge of the network is represented as (0,1), (5,4) etc, implying agents 0 and 1 are connected with each other, agents 5 and 4 are connected with each other. During each time period, all edges are selected sequentially and the agents associated with those edges play the game. We are interested in knowing how the initial state of H/M/L distribution changes as agents interact over a period of time and update their strategy. And how these results change when agents start the game with different initial states (e.g. more H type agents placed with H types or more H type agents placed with M type etc.).
+
+We have considered different combinations of strategies that agents can adopt while taking actions. We assume that agents use perturbed best response implying agents can take action randomly out of H,M or L with a certain positive probability (Young, 2015). At each time when agents require to take action, they look at the strategies of their neighbours and calculate their payoff. All agents calculate their payoffs in the current period and decide if they want to change strategies or stick to what they have been following so far. We have tested four different ways which agents can use to decide what action to take. The "function_to_use" parameter provides details about these and how these are different to each other.
+
+When the simulations are run for "num_of_trials" timeperiod, we get the percentage distribution of  H/M/L which agents used. This shows the percentage of agents who used H/M or L during each time period. The strategy which satisfy the two conditions for norm specified by "norms_agents_frequency" and "norms_time_frequency" are considered as norm. We have looked at two dimensions of norms, number of agents following the norm and for how long it has been followed. We can see the output like below. In below graph, X-axis shows the timeperiod, and Y-axis shows the % of agents who played the respective strategy. Y-axis values are in ratio format (range from 0 - 1), so would need to multiply by 100 to get this in percentage format. 
+
+
+![](https://github.com/ankur-tutlani/multi-agent-decision/raw/main/norm_emergence.png)
+
+
+
+In above figure, strategy "M" satisfies the norm criteria, when we assume "norms_agents_frequency" as 0.7 and "norms_time_frequency" as 0.5. This implies at least 70% of agents following "M" for at least 50% of times. The detailed explanation of the output generated is provided in the next section.
+
+We have also considered the possibility of norm displacement. This is controlled by three parameters, "enable_delta_payoff", "delta_to_add", and "min_time_period" parameters. For norm displacement, we need to specify "enable_delta_payoff" value to "Yes" and also specify a positive/negative value for "delta_to_add" parameter. The "min_time_period" parameter specifies the minimum time period for which the game should run before checking for norm displacement. Its value should be set lower than "num_of_trials" parameter. When any strategy satisfies the norm criteria laid out (say "M"), then the "delta_to_add" value is being added to the payoff values for rest of the other strategies ("H" and "L") after "min_time_period". The revised payoff matrix would be used by agents once the delta value is added to the payoff values. This would continue as long as some other strategy satisfies the norm criteria and the game is still not played for "num_of_trials" timeperiods. If some other strategy now satisfies the norm criteria (say "H"), then the delta payoff value would be added to the rest of the strategies ("M" and "L"). And this process continues till the game is played for all the timeperiods ("num_of_trials"). This can be seen in below figure where "M" strategy is being displaced by "H" strategy after around 40 timeperiods. And then again there is an attempt to displace "H" strategy with "M" strategy later in the game at around 90th timeperiod.
+
+
+![](https://github.com/ankur-tutlani/multi-agent-decision/raw/main/norm_displacement.png)
+
+
+
+## How to interpret output?
+There are total 10 files generated in the output when there is at least 1 strategy which satisfies the norm criteria.
+
+    input_network_ringnetwork_2023-02-02-21-31-34.png
+    networkgraph_initial_state_ringnetwork_2023-02-02-21-31-34.png
+    strategy_trend_ringnetwork_2023-02-02-21-31-34.png
+	network_after_100_timeperiods_ringnetwork_2023-02-02-21-31-34.png
+    normcandidates_ringnetwork_2023-02-02-21-31-34.xlsx
+    time_when_reached_norm_ringnetwork_2023-02-02-21-31-34.xlsx
+	parameters_ringnetwork_2023-02-02-21-31-34.xlsx
+	aggregate_data_detailed_agent_ringnetwork_2023-02-02-21-31-34.xlsx
+    initial_state_considered_ringnetwork_2023-02-02-21-31-34.xlsx
+	payoff_matrices_considered_by_timeperiod_ringnetwork_2023-02-02-21-31-34.xlsx
+    
+
+
+The 4 image files (.png) contain the network graphs and trend graph which is being considered for the simulation. The "input_network_.." file is the input network with which the game is started. "networkgraph_initial_state_...." file shows initial strategy distribution in the ratio specified in "strategy_share" parameter. The "strategy_trend_..." file shows the percent of agents following "H","M" or "L" strategy at each time period during the game. The "network_after_..." file is the network state at the end of game. Agents following the same strategy would be coloured in the same colour in this file.
+
+Norm file "normcandidates_..." shows strategy that satisfies the norm criteria laid out. File "time_when_reached_norm_..." shows the time period number when the specific strategy met the norm criteria. These 2 files are generated only when at least one strategy satisfies the norm criteria. 
+
+Parameters file "parameters_.." lists all the parameters which have been specified in the function call. File "aggregate_data_detailed_.." has the information on percentage of agents who proposed different strategies at each time period during the game. "initial_state_considered_" file shows the initial state with which game is started. In case of norm displacement, "payoff_matrices_considered_.." shows the payoff matrix considered along with time period. When there is more than one row in this file, this shows payoff matrix is being revised during the simulation run. The timeperiod column in this file shows the time period point at which the payoff matrix is revised.
+
+All the file names end with date and time stamp when the function was executed. It also contains information on network structure used like "ringnetwork" or "smallworld" network etc.
+
+
+## References
+1. Young, H.P. "The evolution of social norms" Annual Review of Economics. 2015 (7),pp.359-387
+2. https://pypi.org/project/networkx/ 
+
```

### Comparing `multi-agent-decision-0.2/README.md` & `multi-agent-decision-0.3/README.md`

 * *Files identical despite different names*

### Comparing `multi-agent-decision-0.2/multi_agent_decision/simulation.py` & `multi-agent-decision-0.3/multi_agent_decision/simulation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
+
 import numpy as np   
 import pandas as pd
 from collections import Counter
 import datetime
 import random
 import matplotlib.pyplot as plt
 import networkx as nx
 import string
 from functools import reduce
 import itertools
 
 
 
-dotprod = lambda K, L: reduce(lambda z1, z2: z1+z2, map(lambda x: reduce(lambda x1, x2: x1*x2, x), zip(K, L))) if len(K)==len(L) else 0
-
 
+dotprod = lambda K, L: reduce(lambda z1, z2: z1+z2, map(lambda x: reduce(lambda x1, x2: x1*x2, x), zip(K, L))) if len(K)==len(L) else 0
 
 # 1.random_seed : random seed to reproduce results. Integer
 # 2.iteration_name: give any name for this iterations. String
 # 3.path_to_save_output. the location where output excel files should be saved. String
 # 4.num_strategies : total number of strategies. Integer
 # 5.agent_initial_state : specify the initial state of agents in list format e.g. ['H','M','M'] in case of 3 agents where 1st agent follows 'H' strategy and agents 2 and 3 follow 'M'. List
 # 6.strategy_share. percent distribution of strategies among agents. Must be specified in list. E.g.[0.4,0.4,0.2]. Must add up to 1. Specify in the order of strategies 0,1,2, and so on. List
@@ -64,15 +64,14 @@
 # small_world3: Returns a connected Watts–Strogatz small-world graph.
 # complete: Returns the complete graph.
 # random: Compute a random graph by swapping edges of a given graph.
 # grid2d: Return the 2d grid graph of mxn nodes, each connected to its nearest neighbors.
 
 
 
-
 def perturbed_response1(num_agents,agent_and_strategy_pd2,potential_edges,perturb_ratio,unique_strategies,fixed_agents,fixed_strategy_to_use):
     
     agent_strategy_to_choose=[]
 
     if len(fixed_agents) > 0:
 
         for j in range(num_agents):
@@ -106,36 +105,42 @@
 
                 agent_strategy_to_choose.append(best_response)
 
 
 
     else:
         for j in range(num_agents):
-            check1 = [i for i in potential_edges if i[0] == j]
-            check2 = [i for i in potential_edges if i[1] == j]
-            check1.extend(check2)
-            flat_list1 = list(set([item for sublist in check1 for item in sublist]))
-            data_to_check = agent_and_strategy_pd2.loc[agent_and_strategy_pd2['agent_no'].isin(flat_list1)].reset_index(drop=True)
+            try:
+                check1 = [i for i in potential_edges if i[0] == j]
+                check2 = [i for i in potential_edges if i[1] == j]
+                check1.extend(check2)
+                flat_list1 = list(set([item for sublist in check1 for item in sublist]))
+                data_to_check = agent_and_strategy_pd2.loc[agent_and_strategy_pd2['agent_no'].isin(flat_list1)].reset_index(drop=True)
 
-            if data_to_check.loc[data_to_check['agent_no']==j]['payoff'].values[0] == max(data_to_check['payoff']):
-                xx = data_to_check.loc[data_to_check['agent_no']==j]['strategy'].values[0]
-            else:
-                xx = list(set(data_to_check.loc[(data_to_check['agent_no']!=j) & (data_to_check['payoff']==max(data_to_check['payoff']))]['strategy'].tolist()))
-                xx = random.choices(population=xx,k=1)[0]
+                if data_to_check.loc[data_to_check['agent_no']==j]['payoff'].values[0] == max(data_to_check['payoff']):
+                    xx = data_to_check.loc[data_to_check['agent_no']==j]['strategy'].values[0]
+                else:
+                    xx = list(set(data_to_check.loc[(data_to_check['agent_no']!=j) & (data_to_check['payoff']==max(data_to_check['payoff']))]['strategy'].tolist()))
+                    xx = random.choices(population=xx,k=1)[0]
 
-            non_recommended = [k for k in unique_strategies if k != xx]
+                non_recommended = [k for k in unique_strategies if k != xx]
 
-            if len(non_recommended) > 0:
-                draw2= random.choices(population=non_recommended,k=1)
-                best_response = random.choices(population=[xx,draw2[0]],weights=[1-perturb_ratio,perturb_ratio],k=1)
-                best_response = best_response[0]
-            else:
-                best_response = xx
+                if len(non_recommended) > 0:
+                    draw2= random.choices(population=non_recommended,k=1)
+                    best_response = random.choices(population=[xx,draw2[0]],weights=[1-perturb_ratio,perturb_ratio],k=1)
+                    best_response = best_response[0]
+                else:
+                    best_response = xx
+
+                agent_strategy_to_choose.append(best_response)
+            
+            except:
+                
+                agent_strategy_to_choose.append(agent_and_strategy_pd2.loc[agent_and_strategy_pd2['agent_no']==j]['strategy'].values[0])
 
-            agent_strategy_to_choose.append(best_response)
 
     return agent_strategy_to_choose
 
 
 
 
 def perturbed_response2(num_agents,agent_and_strategy_pd2,potential_edges,perturb_ratio,unique_strategies,fixed_agents,fixed_strategy_to_use):
@@ -175,40 +180,46 @@
                 index_strategy = [index for index,item in enumerate(agent_payoffs) if item == max(agent_payoffs)]
                 agent_choice = random.choices(index_strategy,k=1)[0]
                 agent_strategy_to_choose.append(agent_choice)
 
 
     else:
         for j in range(num_agents):
-            check1 = [i for i in potential_edges if i[0] == j]
-            check2 = [i for i in potential_edges if i[1] == j]
-            check1.extend(check2)
-            flat_list1 = list(set([item for sublist in check1 for item in sublist]))
-            flat_list1.remove(j) ## to get opponent's agents 
-
-            ### this is aggregated data..
-            percent_share_data =agent_and_strategy_pd2.loc[agent_and_strategy_pd2['agent_no'].isin(flat_list1)].reset_index(drop=True)['strategy'].value_counts(normalize=True).to_frame()
-            percent_share_data.columns = ['prob']
-            percent_share_data['strategy'] = percent_share_data.index.values
-            percent_share_data['prob'] = np.round(percent_share_data['prob'],2)
-            prob_opponent_strategy = []
-            for i in unique_strategies: ### should be in 0,1,2,,,, order 
-                try:
-                    xx = percent_share_data.loc[percent_share_data['strategy']==i]['prob'].values[0]
-                except:
-                    xx = 0
-                prob_opponent_strategy.append(xx)
-
-            agent_payoffs=[]
-            for i in unique_strategies:
-                agent_payoffs.append(dotprod(payoff_matrix[i,].tolist(),prob_opponent_strategy))
-
-            index_strategy = [index for index,item in enumerate(agent_payoffs) if item == max(agent_payoffs)]
-            agent_choice = random.choices(index_strategy,k=1)[0]
-            agent_strategy_to_choose.append(agent_choice)
+            try:
+                
+                check1 = [i for i in potential_edges if i[0] == j]
+                check2 = [i for i in potential_edges if i[1] == j]
+                check1.extend(check2)
+                flat_list1 = list(set([item for sublist in check1 for item in sublist]))
+                flat_list1.remove(j) ## to get opponent's agents 
+
+                ### this is aggregated data..
+                percent_share_data =agent_and_strategy_pd2.loc[agent_and_strategy_pd2['agent_no'].isin(flat_list1)].reset_index(drop=True)['strategy'].value_counts(normalize=True).to_frame()
+                percent_share_data.columns = ['prob']
+                percent_share_data['strategy'] = percent_share_data.index.values
+                percent_share_data['prob'] = np.round(percent_share_data['prob'],2)
+                prob_opponent_strategy = []
+                for i in unique_strategies: ### should be in 0,1,2,,,, order 
+                    try:
+                        xx = percent_share_data.loc[percent_share_data['strategy']==i]['prob'].values[0]
+                    except:
+                        xx = 0
+                    prob_opponent_strategy.append(xx)
+
+                agent_payoffs=[]
+                for i in unique_strategies:
+                    agent_payoffs.append(dotprod(payoff_matrix[i,].tolist(),prob_opponent_strategy))
+
+                index_strategy = [index for index,item in enumerate(agent_payoffs) if item == max(agent_payoffs)]
+                agent_choice = random.choices(index_strategy,k=1)[0]
+                agent_strategy_to_choose.append(agent_choice)
+            
+            except:
+                
+                agent_strategy_to_choose.append(agent_and_strategy_pd2.loc[agent_and_strategy_pd2['agent_no']==j]['strategy'].values[0])
 
     return agent_strategy_to_choose
 
 
 
 
 def perturbed_response3(num_agents,agent_and_strategy_pd2,potential_edges,perturb_ratio,unique_strategies,fixed_agents,fixed_strategy_to_use):
@@ -241,32 +252,38 @@
 
                 agent_strategy_to_choose.append(best_response)
 
 
 
     else:
         for j in range(num_agents):
-            check1 = [i for i in potential_edges if i[0] == j]
-            check2 = [i for i in potential_edges if i[1] == j]
-            check1.extend(check2)
-            flat_list1 = list(set([item for sublist in check1 for item in sublist]))
-            data_to_check = agent_and_strategy_pd2.loc[agent_and_strategy_pd2['agent_no'].isin(flat_list1)].reset_index(drop=True)
+            try:
+                
+                check1 = [i for i in potential_edges if i[0] == j]
+                check2 = [i for i in potential_edges if i[1] == j]
+                check1.extend(check2)
+                flat_list1 = list(set([item for sublist in check1 for item in sublist]))
+                data_to_check = agent_and_strategy_pd2.loc[agent_and_strategy_pd2['agent_no'].isin(flat_list1)].reset_index(drop=True)
+
+                if data_to_check.loc[data_to_check['agent_no']==j]['payoff'].values[0] == max(data_to_check['payoff']):
+                    xx = data_to_check.loc[data_to_check['agent_no']==j]['strategy'].values[0]
+                else:
+                    xx = list(set(data_to_check.loc[(data_to_check['agent_no']!=j) & (data_to_check['payoff']==max(data_to_check['payoff']))]['strategy'].tolist()))
+                    xx = random.choices(population=xx,k=1)[0]
 
-            if data_to_check.loc[data_to_check['agent_no']==j]['payoff'].values[0] == max(data_to_check['payoff']):
-                xx = data_to_check.loc[data_to_check['agent_no']==j]['strategy'].values[0]
-            else:
-                xx = list(set(data_to_check.loc[(data_to_check['agent_no']!=j) & (data_to_check['payoff']==max(data_to_check['payoff']))]['strategy'].tolist()))
-                xx = random.choices(population=xx,k=1)[0]
 
+                draw2= random.choices(population=unique_strategies,k=1)
+                best_response = random.choices(population=[xx,draw2[0]],weights=[1-perturb_ratio,perturb_ratio],k=1)
+                best_response = best_response[0]
 
-            draw2= random.choices(population=unique_strategies,k=1)
-            best_response = random.choices(population=[xx,draw2[0]],weights=[1-perturb_ratio,perturb_ratio],k=1)
-            best_response = best_response[0]
+                agent_strategy_to_choose.append(best_response)
+            
+            except:
+                agent_strategy_to_choose.append(agent_and_strategy_pd2.loc[agent_and_strategy_pd2['agent_no']==j]['strategy'].values[0])
 
-            agent_strategy_to_choose.append(best_response)
 
     return agent_strategy_to_choose
 
 
 
 
 def perturbed_response4(num_agents,agent_and_strategy_pd2,potential_edges,fixed_agents,fixed_strategy_to_use):
@@ -289,29 +306,31 @@
                 if data_to_check.loc[data_to_check['agent_no']==j]['payoff'].values[0] == max(data_to_check['payoff']):
                     agent_strategy_to_choose.append(data_to_check.loc[data_to_check['agent_no']==j]['strategy'].values[0])
                 else:
                     xx = list(set(data_to_check.loc[(data_to_check['agent_no']!=j) & (data_to_check['payoff']==max(data_to_check['payoff']))]['strategy'].tolist()))
                     agent_strategy_to_choose.append(random.choices(population=xx,k=1)[0])
 
     else:
-
         for j in range(num_agents):
+            try:
+                check1 = [i for i in potential_edges if i[0] == j]
+                check2 = [i for i in potential_edges if i[1] == j]
+                check1.extend(check2)
+                flat_list1 = list(set([item for sublist in check1 for item in sublist]))
+                data_to_check = agent_and_strategy_pd2.loc[agent_and_strategy_pd2['agent_no'].isin(flat_list1)].reset_index(drop=True)
 
-            check1 = [i for i in potential_edges if i[0] == j]
-            check2 = [i for i in potential_edges if i[1] == j]
-            check1.extend(check2)
-            flat_list1 = list(set([item for sublist in check1 for item in sublist]))
-            data_to_check = agent_and_strategy_pd2.loc[agent_and_strategy_pd2['agent_no'].isin(flat_list1)].reset_index(drop=True)
-
-            if data_to_check.loc[data_to_check['agent_no']==j]['payoff'].values[0] == max(data_to_check['payoff']):
-                agent_strategy_to_choose.append(data_to_check.loc[data_to_check['agent_no']==j]['strategy'].values[0])
-            else:
-                xx = list(set(data_to_check.loc[(data_to_check['agent_no']!=j) & (data_to_check['payoff']==max(data_to_check['payoff']))]['strategy'].tolist()))
-                agent_strategy_to_choose.append(random.choices(population=xx,k=1)[0])
-
+                if data_to_check.loc[data_to_check['agent_no']==j]['payoff'].values[0] == max(data_to_check['payoff']):
+                    agent_strategy_to_choose.append(data_to_check.loc[data_to_check['agent_no']==j]['strategy'].values[0])
+                else:
+                    xx = list(set(data_to_check.loc[(data_to_check['agent_no']!=j) & (data_to_check['payoff']==max(data_to_check['payoff']))]['strategy'].tolist()))
+                    agent_strategy_to_choose.append(random.choices(population=xx,k=1)[0])
+                    
+            except:
+                agent_strategy_to_choose.append(agent_and_strategy_pd2.loc[agent_and_strategy_pd2['agent_no']==j]['strategy'].values[0])
+                
     return agent_strategy_to_choose
 
 
 
 
 def simulation_function_neighbors(random_seed,
                                  iteration_name,
@@ -376,25 +395,25 @@
     list_to_fill = []
     for i in range(num_strategies):
         list_to_fill.append([i]*round(strategy_share[i]*num_agents))
         
     flat_list = [item for sublist in list_to_fill for item in sublist]
     if len(flat_list) == num_agents:
         pass
-    #         print("ok")
+    
     elif len(flat_list) < num_agents:
         delta = num_agents - len(flat_list)
         for kk in range(delta):
             flat_list.append(flat_list[-1])
-    #         print("last elements added")
+   
     else:
         delta = len(flat_list) - num_agents
         for kk in range(delta):
             flat_list.pop()
-    #         print("last elements deleted")
+    
 
     if len(agent_initial_state) > 0:
         samplelist1 = agent_initial_state
     else:
         samplelist1 = random.sample(flat_list,len(flat_list))
     
     
@@ -418,29 +437,33 @@
     
     nx.draw(G,with_labels=True)
     plt.savefig(path_to_save_output+"input_network_"+iteration_name+"_"+today+".png")
     plt.clf()
     
     potential_edges = list(G.edges)
     
+    agents_in_edges = list(set([i[0] for i in potential_edges]+[i[1] for i in potential_edges]))
+    agents_in_network = list(range(num_agents))
+    delta_agents_hardcoded = [i for i in agents_in_network if i not in agents_in_edges]
+    
     agents_list = list(range(num_agents))
     agent_and_strategy_pd = pd.DataFrame({'agent_no':agents_list,'strategy':samplelist1})
     intial_states_pd = pd.DataFrame([{'initial_state':str([thisdict[k] for k in samplelist1])}],columns=['initial_state'])
     
     
     trend_db_to_store = pd.DataFrame(columns=["percent_count","strategy","timeperiod_number","starting_position"])
     payoff_matrices = []
     payoff_matrices.append(str(payoff_matrix))
     payoff_matrices_timeperiod = []
     payoff_matrices_timeperiod.append(0)
     agent_and_strategy_pd['timeperiod_number'] = 0
     unique_strategies = list(range(num_strategies))
     
     
-    ### initial state graph
+    
     names_to_check=unique_strategies
     get_colors = lambda n: list(map(lambda i: "#" + "%06x" % random.randint(0, 0xFFFFFF),range(n)))
     list_of_colors = get_colors(len(names_to_check))
     color_map = []
     for j in range(len(samplelist1)):
         for i in range(len(names_to_check)):
             if samplelist1[j] == names_to_check[i]:
@@ -457,25 +480,28 @@
     plt.clf()
     
     for timeperiod in range(1,num_of_trials+1):
         payoff_matrix_original = payoff_matrix.copy()
 
         agent_payoffs_to_store = []  
         for j in range(num_agents):
-            check1 = [i for i in potential_edges if i[0] == j]
-            check2 = [i for i in potential_edges if i[1] == j]
-            check1.extend(check2)
-            flat_list1 = list(set([item for sublist in check1 for item in sublist]))
-            flat_list1.remove(j)
-            row_strategy = agent_and_strategy_pd.loc[agent_and_strategy_pd['agent_no'] == j]['strategy'].values[0]
-            data_to_check = agent_and_strategy_pd.loc[agent_and_strategy_pd['agent_no'].isin(flat_list1)].reset_index(drop=True)
-            agent_payoff = 0
-            for i in range(len(data_to_check)):
-                agent_payoff += payoff_matrix[row_strategy,data_to_check.iloc[i]['strategy']] 
-            agent_payoffs_to_store.append(agent_payoff)
+            try:
+                check1 = [i for i in potential_edges if i[0] == j]
+                check2 = [i for i in potential_edges if i[1] == j]
+                check1.extend(check2)
+                flat_list1 = list(set([item for sublist in check1 for item in sublist]))
+                flat_list1.remove(j)
+                row_strategy = agent_and_strategy_pd.loc[agent_and_strategy_pd['agent_no'] == j]['strategy'].values[0]
+                data_to_check = agent_and_strategy_pd.loc[agent_and_strategy_pd['agent_no'].isin(flat_list1)].reset_index(drop=True)
+                agent_payoff = 0
+                for i in range(len(data_to_check)):
+                    agent_payoff += payoff_matrix[row_strategy,data_to_check.iloc[i]['strategy']] 
+                agent_payoffs_to_store.append(agent_payoff)
+            except:
+                agent_payoffs_to_store.append(None)
 
 
         agent_and_strategy_payoff = pd.DataFrame({'agent_no':agents_list,'payoff':agent_payoffs_to_store})
         agent_and_strategy_pd2 = pd.merge(agent_and_strategy_pd,agent_and_strategy_payoff,on='agent_no')
 
         if function_to_use == 'perturbed_response1':
             agent_strategy_to_choose = perturbed_response1(num_agents,agent_and_strategy_pd2,potential_edges,perturb_ratio,unique_strategies,fixed_agents,fixed_strategy_to_use)
@@ -491,17 +517,17 @@
 
         data1_to_store = agent_and_strategy_pd['strategy'].value_counts(normalize=True).to_frame()
         data1_to_store.columns = ['percent_count']
         data1_to_store['strategy'] = data1_to_store.index.tolist()
         data1_to_store = data1_to_store.replace({"strategy":thisdict})
         data1_to_store["timeperiod_number"] = timeperiod
         data1_to_store["starting_position"] = str([thisdict[k] for k in samplelist1])
-        trend_db_to_store = trend_db_to_store.append(data1_to_store,ignore_index=True)
+        trend_db_to_store = pd.concat([trend_db_to_store,data1_to_store],ignore_index=True)
 
-        #### added ###
+        
         if enable_delta_payoff == 'Yes' and timeperiod > min_time_period and max(trend_db_to_store['percent_count']) >= norms_agents_frequency:
             norms_to_store = []
             percent_time_frequency = []
             norms_candidates = trend_db_to_store.loc[trend_db_to_store['percent_count']>= norms_agents_frequency]
             norms_candidates = norms_candidates.replace({'strategy':thisdict2}) ### convert to numeric.
             potential_norms_candidate = np.unique(norms_candidates['strategy']).tolist()
             for k in potential_norms_candidate:
@@ -531,19 +557,19 @@
                     payoff_matrices_timeperiod.append(timeperiod)
 
 
     payoff_matrices_pd = pd.DataFrame(payoff_matrices)
     payoff_matrices_pd.columns = ['payoff_matrix']
     payoff_matrices_pd['timeperiod'] = payoff_matrices_timeperiod
     
-    #### strategy converted to norm ####
+    
     norms_to_store = []
     percent_time_frequency = []
     norms_candidates = trend_db_to_store.loc[trend_db_to_store['percent_count']>= norms_agents_frequency]
-    # norms_candidates = norms_candidates.replace({'strategy':thisdict2}) ### convert to numeric.
+    
     potential_norms_candidate = np.unique(norms_candidates['strategy']).tolist()
     for k in potential_norms_candidate:
         norms_candidates2 = norms_candidates.loc[norms_candidates['strategy']==k]
         distinct_timeperiod = len(np.unique(norms_candidates2['timeperiod_number']))
         norms_candidates2 = round(distinct_timeperiod/len(np.unique(trend_db_to_store['timeperiod_number'])),2)
         if norms_candidates2 >= norms_time_frequency:
             norms_to_store.append(k)
@@ -557,51 +583,62 @@
         if len(norms_candidates2) > 0:
             norms_candidates2.to_excel(path_to_save_output+"normcandidates_"+iteration_name+"_"+today+".xlsx",index=None)
     except:
         pass
     
     
     
-    ##### distribution at the end of timeperiod.
+    
     color_map = []
     for j in range(len(agent_strategy_to_choose)):
         for i in range(len(names_to_check)):
             if agent_strategy_to_choose[j] == names_to_check[i]:
                 color_map.append(list_of_colors[i])
 
     for i in range(len(G)):
         G.nodes[i]["name_offered"] = [thisdict[k] for k in agent_strategy_to_choose][i]
 
     labels_for_graph = nx.get_node_attributes(G,"name_offered")
     nx.draw(G,with_labels=True,node_color=color_map,labels=labels_for_graph)
     l,r = plt.xlim()
     plt.xlim(l-0.05,r+0.05)
-    # plt.show()
+    
     plt.savefig(path_to_save_output+"network_after_"+str(num_of_trials)+'_timeperiods_'+iteration_name+"_"+today+".png")
     plt.clf()
     
     
-    ###  trend graph
+    
     fig,ax = plt.subplots()
     data_for_trend_plot = trend_db_to_store.loc[trend_db_to_store['starting_position']==str([thisdict[k] for k in samplelist1])]
     data_for_trend_plot = data_for_trend_plot.reset_index(drop=True)
     for label,grp in data_for_trend_plot.groupby('strategy'):
         grp.plot(x='timeperiod_number',y='percent_count',ax=ax,label=label)
+    
+    
+    x_values11 = data_for_trend_plot['timeperiod_number'].unique()
+    total_periods11 = len(x_values11)
+    max_display_labels = 5  
+    interval11 = max(1, total_periods11 // max_display_labels)  
+
+    ax.set_xticks(np.arange(len(x_values11))[::interval11])
+    ax.set_xticklabels(x_values11[::interval11])
+    
+    
     ax.set_xlabel('Timeperiod')
     ax.set_ylabel('Count %')
-    # plt.show()
+    
     plt.savefig(path_to_save_output+"strategy_trend_"+iteration_name+"_"+today+".png")
     plt.clf()
     
     
-    ###### dataframe of strategy the timeperiod when it reached the norms stage #####
+    
     db_to_fill2 = pd.DataFrame()
     db_to_fill2["timeperiod"] = -1
     db_to_fill2["name_offered"] = -1
-    # data_for_norms_plot = trend_db_to_store.loc[trend_db_to_store['starting_position']==str([thisdict[k] for k in samplelist1])]
+    
     if len(norms_to_store) > 0:
         for j in norms_to_store:
             foocheck = data_for_trend_plot.loc[data_for_trend_plot["strategy"]==j]
             foocheck = foocheck.loc[foocheck['percent_count']>= norms_agents_frequency].reset_index(drop=True)
             foocheck = foocheck.sort_values(["timeperiod_number"])
             foocheck["count_names_offered"] = (foocheck["strategy"]==j).cumsum()
             foocheck["cum_perc"] = foocheck["count_names_offered"]/len(np.unique(data_for_trend_plot['timeperiod_number']))
@@ -640,7 +677,8 @@
     parameters_pd["parameter"]=parameters_pd.index
     parameters_pd[["parameter","parameter_values"]].to_excel(path_to_save_output+"parameters_"+iteration_name+"_"+today+".xlsx",index=None)
     
     intial_states_pd.to_excel(path_to_save_output+"initial_state_considered_"+iteration_name+"_"+today+".xlsx",index=None)
     payoff_matrices_pd.to_excel(path_to_save_output+"payoff_matrices_considered_by_timeperiod_"+iteration_name+"_"+today+".xlsx",index=None)
 
     return(print("done"))
+
```

### Comparing `multi-agent-decision-0.2/multi_agent_decision.egg-info/PKG-INFO` & `multi-agent-decision-0.3/multi_agent_decision.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,189 +1,189 @@
 Metadata-Version: 2.1
 Name: multi-agent-decision
-Version: 0.2
+Version: 0.3
 Summary: Simulates the actions which agents take under multi-agent systems and social networks
 Home-page: https://github.com/ankur-tutlani/multi-agent-decision
+Download-URL: https://github.com/ankur-tutlani/multi_agent_decision/archive/refs/tags/v_03.tar.gz
 Author: ankurtutlani
 Author-email: ankur.tutlani@gmail.com
 License: MIT
-Download-URL: https://github.com/ankur-tutlani/multi_agent_decision/archive/refs/tags/v_02.tar.gz
-Description: 
-        # Decision-making under Multi-Agent Systems and Social Networks
-        
-        This library is used to ascertain how agents take decisions under multi-agent systems. Agents are connected with other agents via a social network and play symmetric games. Agents take decisions based upon their interactions with other agents in the neighbourhood. The strategy which is being played most frequently by agents and for a longer duration of time is a potential candidate for being called a norm. This library demonstrates how norms evolve from bottom-up when agents interact with other agents and decide what is best for them.
-        
-        
-        ## How to use it?
-        
-        
-        ```bash
-          # Install
-          pip install multi-agent-decision
-        
-          
-          # Import
-          from multi_agent_decision import simulation
-        
-          # Execute 
-          simulation.simulation_function_neighbors(random_seed = 226822,
-                                         iteration_name = "test1",
-                                         path_to_save_output = "C:\\Users\\Downloads\\",
-                                         num_strategies=3,
-                                         agent_initial_state =[],
-                                         strategy_share = [0.4,0.4,0.2],
-                                         strategy_pair = {0: "H",1: "M",2: "L"},
-                                         payoff_values = [[0,0,70],[0,50,50],[30,30,30]],
-                                         network_name = "small_world1",
-                                         prob_edge_rewire = 0.50,
-                                         grid_network_m = 5,
-                                         grid_network_n = 8,
-                                         num_agents = 20, 
-                                         num_neighbors = 2,
-                                         delta_to_add = 20,
-                                         norms_agents_frequency = 0.7,
-                                         norms_time_frequency = 0.5,
-                                         min_time_period = 20,
-                                         enable_delta_payoff = "Yes",
-                                         num_of_trials = 50,
-                                         fixed_agents = [5,9],
-                                         fixed_strategy_to_use = 0,
-                                         function_to_use = "perturbed_response4",
-                                         perturb_ratio = 0.05
-                                          
-                                         )
-        
-        
-        ```
-            
-        ## Function parameters
-        Following are the parameters which are required to be specified. At the end in the parenthesis, it shows the data type of the parameter which is required or the possible values which is required to be used. In following we will use agents' strategies, actions, choices, responses interchangeably. These all represent same intent and meaning in our context.  
-        
-        1. random_seed : Random seed to reproduce results. (Integer)
-        2. iteration_name: Give any name for this iteration. (String)
-        3. path_to_save_output : The location where output excel files should be saved. (String)
-        4. num_strategies : Total number of strategies. (Integer)
-        5. agent_initial_state : Specify the initial state of agents in list format e.g. ["H","M","M"] in case of 3 agents where 1st agent follows "H" strategy and agents 2 and 3 follow "M". (List)
-        6. strategy_share : Percent distribution of strategies among agents. Must be specified in list format. E.g.[0.4,0.4,0.2]. Must add up to 1. Specify in the order of strategies 0,1,2, and so on. (List)
-        7. strategy_pair : Strategy pair in dictionary format. E.g. {0: "H",1: "M",2: "L"}. 0 strategy is "H", 1 strategy is "M", and so on. Count must match with num_strategies argument. Keys would need to be 0,1,2, etc. Value corresponding to keys can be anything in string format. (Dict)
-        8. payoff_values : List of payoff values. E.g. [[0,0,70],[0,50,50],[30,30,30]]. The first list [0,0,70] is the first row of the 3*3 payoff matrix assuming we have 3 strategies. Second list [0,50,50] is the second row of the payoff matrix and third list [30,30,30] is the third row of payoff matrix.(List)
-        9. network_name : Specify one of these values. A detailed explanation is provided below. ["small_world1","small_world2","small_world3","complete","random","grid2d"]. (String)
-        10. prob_edge_rewire : Small world network parameter. Probability of rewiring existing edges or adding new edges. (Float)
-        11. grid_network_m :  2-dimensional grid network parameter. Number of nodes. (Integer)
-        12. grid_network_n :  2-dimensional grid network parameter. Number of nodes. (Integer)
-        13. num_agents : Number of agents. (Integer)
-        14. num_neighbors : Number of neighbours. (Integer)
-        15. delta_to_add : Delta payoff value which will be added (or deducted in case of negative value) to the payoffs in case of norm displacement. (Float/Integer)
-        16. norms_agents_frequency : Norm condition. Minimum percentage of agents required to use same strategy. Specify number from 0 (0% agents) to 1(100% agents). (Float)
-        17. norms_time_frequency : Norm condition. Minimum percentage of times agents require to use same strategy. Specify number from 0 (no time period) to 1 (all time periods). (Float)
-        18. min_time_period : Minimum time period for which the game should be run before adding delta payoff. (Integer)
-        19. enable_delta_payoff : If norm displacement is required to be assessed , specify "Yes" else specify "No".
-        20. num_of_trials : Number of trials, how long game should run. (Integer)
-        21. fixed_agents : Agents assumed as fixed. e.g. [2,3] shows we want agents 2 and 3 to be fixed. (List)
-        22. fixed_strategy_to_use : Specify key value from strategy_pair. e.g. if we want fixed agents to follow strategy "H" and strategy_pair is {0: "H",1: "M",2: "L"}, specify the value as 0. (Integer)
-        23. function_to_use : Specify one of these values. A detailed explanation is provided below. ["perturbed_response1","perturbed_response2","perturbed_response3","perturbed_response4"]. (String)
-        24. perturb_ratio : Probability of agents taking action randomly. (Float)
-        
-        
-        <br />
-        
-        In the "function_to_use" parameter above, below is the explanation for what these different values mean inside the list specified above.
-        
-        1. perturbed_response1: Agents select the best response (1-perturb_ratio)*100% times among the strategies which are most frequently used. If there is more than one such strategy, then agents select any one strategy randomly. Agents select random strategy (perturb_ratio)*100% times among the strategies which are not most frequently used. Here also, if there is more than one such strategy, then agents select any one strategy randomly out of these.
-        2. perturbed_response2: Agent selects strategy randomly according to the relative weightage of different strategies. These relative weights are the % of times the respective strategy has been used by opponents in the past. 
-        3. perturbed_response3: This is same as "perturbed_response1" function except agent selects random strategy (perturb_ratio)*100% times from all the possible strategies and not only from the ones which were not used most frequently by their opponents.
-        4. perturbed_response4: Agent selects the best response 100% of times among the strategies which are most frequently used. If there is more than one such strategy, then agents select any one strategy randomly. There is no perturbation element (perturb_ratio is considered as zero).
-        
-        
-        <br/>
-        
-        In the "network_name" parameter above, below is the explanation for what these different values mean inside the list specified above.
-        1. small_world1: Returns a Watts Strogatz small-world graph. Here number of edges remained constant once we increase the prob_edge_rewire value. Shortcut edges if added would replace the existing ones. But total count of edges remained constant.
-        2. small_world2: Returns a Newman Watts Strogatz small-world graph. Here number of edges increased once we increase the prob_edge_rewire value. It would add more shortcut edges in addition to what already exist.
-        3. small_world3: Returns a connected Watts Strogatz small-world graph. Rest of the explanation remains as small_world1.
-        4. complete: Returns the complete graph.
-        5. random: Compute a random graph by swapping edges of a given graph. The given graph used is Watts Strogatz small-world graph (the one produced by "small_world1").
-        6. grid2d: Return the 2d grid graph of mxn nodes, each connected to its nearest neighbors.
-        
-        We have used the networkx python library to populate these graphs. For more information around these graphs and how these are produced please refer to the link in the reference section.
-        
-        
-        
-        ## Function explanation
-        Here we explain the underlying functioning of this library with the help of an example. But this can be replicated to any symmetric game wherein we have defined finite strategies along with its payoff values.
-        
-        We assume there is a Nash demand game wherein each agent can make 3 demands, High (70), Medium (50) or Low (30). The rule of the game is if the total demands made by two agents in any given iteration are more than 100, no one is going to get anything. Below is the payoff matrix of row versus column player looks like.
-        
-        		  H	  M	    L
-            H	(0,0)	(0,0)	 (70,30)
-            M	(0,0)	(50,50)	 (50,30)
-            L	(30,70)	(30,50)	 (30,30)
-        	
-        
-        There are 3 pure strategy Nash equilibria, (H, L), (M, M) and (L, H). There is not a strictly or weakly dominant strategy for any of the row or column player. Suppose that agents are connected in a ring network wherein each agent is connected with two other agents, one on the left and one on the right like in below image.
-        
-        
-        ![](https://github.com/ankur-tutlani/multi-agent-decision/raw/main/network_graph.png)
-        
-        
-        Agents update their strategy if any of their neighbours (defined by "num_neighbors") are having higher payoff else, they stick to their own strategy which they have been following. Payoffs are computed as follows. If agent with strategy H meets agent with strategy M and L, then payoff from meeting with strategy M agent equals 0 and payoff from meeting with strategy L agent equals 70, hence the total payoff equals 70. In case of a tie, meaning payoffs are exactly same following current strategy versus payoffs from neighbours" strategy then agents stick to the strategy which they have been following. 
-        
-        We assume agents are distributed in a specific ratio in a network. E.g., if total agents ("num_agents") are 20 and if they are distributed in 40/40/20 distribution ("strategy_share"), that implies there are 8 H type agents, 8 M type agents and 4 L type agents. This can be represented in a list format like this [H,H,H,H,H,H,H,H,M,M,M,M,M,M,M,M,L,L,L,L]. This list shows first agent follows "H" (first value from the left), last agent follows "L" (last value from the right), agent 16 follows "M" etc.This list can be rearranged in multiple ways but still satisfies the condition of 40/40/20. Hence, we require to specify initial state of the agents in "agent_initial_state" parameter in the list format. If this parameter is empty, the function will select any one state randomly. This initial state is being shown in "initial_state_considered_..."  excel file output. For more details on the output generated, please refer to the section below.
-        
-        We start the game with one edge of the network is selected at any given point. Edge of the network is represented as (0,1), (5,4) etc, implying agents 0 and 1 are connected with each other, agents 5 and 4 are connected with each other. During each time period, all edges are selected sequentially and the agents associated with those edges play the game. We are interested in knowing how the initial state of H/M/L distribution changes as agents interact over a period of time and update their strategy. And how these results change when agents start the game with different initial states (e.g. more H type agents placed with H types or more H type agents placed with M type etc.).
-        
-        We have considered different combinations of strategies that agents can adopt while taking actions. We assume that agents use perturbed best response implying agents can take action randomly out of H,M or L with a certain positive probability (Young, 2015). At each time when agents require to take action, they look at the strategies of their neighbours and calculate their payoff. All agents calculate their payoffs in the current period and decide if they want to change strategies or stick to what they have been following so far. We have tested four different ways which agents can use to decide what action to take. The "function_to_use" parameter provides details about these and how these are different to each other.
-        
-        When the simulations are run for "num_of_trials" timeperiod, we get the percentage distribution of  H/M/L which agents used. This shows the percentage of agents who used H/M or L during each time period. The strategy which satisfy the two conditions for norm specified by "norms_agents_frequency" and "norms_time_frequency" are considered as norm. We have looked at two dimensions of norms, number of agents following the norm and for how long it has been followed. We can see the output like below. In below graph, X-axis shows the timeperiod, and Y-axis shows the % of agents who played the respective strategy. Y-axis values are in ratio format (range from 0 - 1), so would need to multiply by 100 to get this in percentage format. 
-        
-        
-        ![](https://github.com/ankur-tutlani/multi-agent-decision/raw/main/norm_emergence.png)
-        
-        
-        
-        In above figure, strategy "M" satisfies the norm criteria, when we assume "norms_agents_frequency" as 0.7 and "norms_time_frequency" as 0.5. This implies at least 70% of agents following "M" for at least 50% of times. The detailed explanation of the output generated is provided in the next section.
-        
-        We have also considered the possibility of norm displacement. This is controlled by three parameters, "enable_delta_payoff", "delta_to_add", and "min_time_period" parameters. For norm displacement, we need to specify "enable_delta_payoff" value to "Yes" and also specify a positive/negative value for "delta_to_add" parameter. The "min_time_period" parameter specifies the minimum time period for which the game should run before checking for norm displacement. Its value should be set lower than "num_of_trials" parameter. When any strategy satisfies the norm criteria laid out (say "M"), then the "delta_to_add" value is being added to the payoff values for rest of the other strategies ("H" and "L") after "min_time_period". The revised payoff matrix would be used by agents once the delta value is added to the payoff values. This would continue as long as some other strategy satisfies the norm criteria and the game is still not played for "num_of_trials" timeperiods. If some other strategy now satisfies the norm criteria (say "H"), then the delta payoff value would be added to the rest of the strategies ("M" and "L"). And this process continues till the game is played for all the timeperiods ("num_of_trials"). This can be seen in below figure where "M" strategy is being displaced by "H" strategy after around 40 timeperiods. And then again there is an attempt to displace "H" strategy with "M" strategy later in the game at around 90th timeperiod.
-        
-        
-        ![](https://github.com/ankur-tutlani/multi-agent-decision/raw/main/norm_displacement.png)
-        
-        
-        
-        ## How to interpret output?
-        There are total 10 files generated in the output when there is at least 1 strategy which satisfies the norm criteria.
-        
-            input_network_ringnetwork_2023-02-02-21-31-34.png
-            networkgraph_initial_state_ringnetwork_2023-02-02-21-31-34.png
-            strategy_trend_ringnetwork_2023-02-02-21-31-34.png
-        	network_after_100_timeperiods_ringnetwork_2023-02-02-21-31-34.png
-            normcandidates_ringnetwork_2023-02-02-21-31-34.xlsx
-            time_when_reached_norm_ringnetwork_2023-02-02-21-31-34.xlsx
-        	parameters_ringnetwork_2023-02-02-21-31-34.xlsx
-        	aggregate_data_detailed_agent_ringnetwork_2023-02-02-21-31-34.xlsx
-            initial_state_considered_ringnetwork_2023-02-02-21-31-34.xlsx
-        	payoff_matrices_considered_by_timeperiod_ringnetwork_2023-02-02-21-31-34.xlsx
-            
-        
-        
-        The 4 image files (.png) contain the network graphs and trend graph which is being considered for the simulation. The "input_network_.." file is the input network with which the game is started. "networkgraph_initial_state_...." file shows initial strategy distribution in the ratio specified in "strategy_share" parameter. The "strategy_trend_..." file shows the percent of agents following "H","M" or "L" strategy at each time period during the game. The "network_after_..." file is the network state at the end of game. Agents following the same strategy would be coloured in the same colour in this file.
-        
-        Norm file "normcandidates_..." shows strategy that satisfies the norm criteria laid out. File "time_when_reached_norm_..." shows the time period number when the specific strategy met the norm criteria. These 2 files are generated only when at least one strategy satisfies the norm criteria. 
-        
-        Parameters file "parameters_.." lists all the parameters which have been specified in the function call. File "aggregate_data_detailed_.." has the information on percentage of agents who proposed different strategies at each time period during the game. "initial_state_considered_" file shows the initial state with which game is started. In case of norm displacement, "payoff_matrices_considered_.." shows the payoff matrix considered along with time period. When there is more than one row in this file, this shows payoff matrix is being revised during the simulation run. The timeperiod column in this file shows the time period point at which the payoff matrix is revised.
-        
-        All the file names end with date and time stamp when the function was executed. It also contains information on network structure used like "ringnetwork" or "smallworld" network etc.
-        
-        
-        ## References
-        1. Young, H.P. "The evolution of social norms" Annual Review of Economics. 2015 (7),pp.359-387
-        2. https://pypi.org/project/networkx/ 
-        
-        
 Keywords: game theory,evolutionary game,social norms,multi-agent systems,evolution,social network,computational economics,simulation,agent-based modeling,computation
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+
+# Decision-making under Multi-Agent Systems and Social Networks
+
+This library is used to ascertain how agents take decisions under multi-agent systems. Agents are connected with other agents via a social network and play symmetric games. Agents take decisions based upon their interactions with other agents in the neighbourhood. The strategy which is being played most frequently by agents and for a longer duration of time is a potential candidate for being called a norm. This library demonstrates how norms evolve from bottom-up when agents interact with other agents and decide what is best for them.
+
+
+## How to use it?
+
+
+```bash
+  # Install
+  pip install multi-agent-decision
+
+  
+  # Import
+  from multi_agent_decision import simulation
+
+  # Execute 
+  simulation.simulation_function_neighbors(random_seed = 226822,
+                                 iteration_name = "test1",
+                                 path_to_save_output = "C:\\Users\\Downloads\\",
+                                 num_strategies=3,
+                                 agent_initial_state =[],
+                                 strategy_share = [0.4,0.4,0.2],
+                                 strategy_pair = {0: "H",1: "M",2: "L"},
+                                 payoff_values = [[0,0,70],[0,50,50],[30,30,30]],
+                                 network_name = "small_world1",
+                                 prob_edge_rewire = 0.50,
+                                 grid_network_m = 5,
+                                 grid_network_n = 8,
+                                 num_agents = 20, 
+                                 num_neighbors = 2,
+                                 delta_to_add = 20,
+                                 norms_agents_frequency = 0.7,
+                                 norms_time_frequency = 0.5,
+                                 min_time_period = 20,
+                                 enable_delta_payoff = "Yes",
+                                 num_of_trials = 50,
+                                 fixed_agents = [5,9],
+                                 fixed_strategy_to_use = 0,
+                                 function_to_use = "perturbed_response4",
+                                 perturb_ratio = 0.05
+                                  
+                                 )
+
+
+```
+    
+## Function parameters
+Following are the parameters which are required to be specified. At the end in the parenthesis, it shows the data type of the parameter which is required or the possible values which is required to be used. In following we will use agents' strategies, actions, choices, responses interchangeably. These all represent same intent and meaning in our context.  
+
+1. random_seed : Random seed to reproduce results. (Integer)
+2. iteration_name: Give any name for this iteration. (String)
+3. path_to_save_output : The location where output excel files should be saved. (String)
+4. num_strategies : Total number of strategies. (Integer)
+5. agent_initial_state : Specify the initial state of agents in list format e.g. ["H","M","M"] in case of 3 agents where 1st agent follows "H" strategy and agents 2 and 3 follow "M". (List)
+6. strategy_share : Percent distribution of strategies among agents. Must be specified in list format. E.g.[0.4,0.4,0.2]. Must add up to 1. Specify in the order of strategies 0,1,2, and so on. (List)
+7. strategy_pair : Strategy pair in dictionary format. E.g. {0: "H",1: "M",2: "L"}. 0 strategy is "H", 1 strategy is "M", and so on. Count must match with num_strategies argument. Keys would need to be 0,1,2, etc. Value corresponding to keys can be anything in string format. (Dict)
+8. payoff_values : List of payoff values. E.g. [[0,0,70],[0,50,50],[30,30,30]]. The first list [0,0,70] is the first row of the 3*3 payoff matrix assuming we have 3 strategies. Second list [0,50,50] is the second row of the payoff matrix and third list [30,30,30] is the third row of payoff matrix.(List)
+9. network_name : Specify one of these values. A detailed explanation is provided below. ["small_world1","small_world2","small_world3","complete","random","grid2d"]. (String)
+10. prob_edge_rewire : Small world network parameter. Probability of rewiring existing edges or adding new edges. (Float)
+11. grid_network_m :  2-dimensional grid network parameter. Number of nodes. (Integer)
+12. grid_network_n :  2-dimensional grid network parameter. Number of nodes. (Integer)
+13. num_agents : Number of agents. (Integer)
+14. num_neighbors : Number of neighbours. (Integer)
+15. delta_to_add : Delta payoff value which will be added (or deducted in case of negative value) to the payoffs in case of norm displacement. (Float/Integer)
+16. norms_agents_frequency : Norm condition. Minimum percentage of agents required to use same strategy. Specify number from 0 (0% agents) to 1(100% agents). (Float)
+17. norms_time_frequency : Norm condition. Minimum percentage of times agents require to use same strategy. Specify number from 0 (no time period) to 1 (all time periods). (Float)
+18. min_time_period : Minimum time period for which the game should be run before adding delta payoff. (Integer)
+19. enable_delta_payoff : If norm displacement is required to be assessed , specify "Yes" else specify "No".
+20. num_of_trials : Number of trials, how long game should run. (Integer)
+21. fixed_agents : Agents assumed as fixed. e.g. [2,3] shows we want agents 2 and 3 to be fixed. (List)
+22. fixed_strategy_to_use : Specify key value from strategy_pair. e.g. if we want fixed agents to follow strategy "H" and strategy_pair is {0: "H",1: "M",2: "L"}, specify the value as 0. (Integer)
+23. function_to_use : Specify one of these values. A detailed explanation is provided below. ["perturbed_response1","perturbed_response2","perturbed_response3","perturbed_response4"]. (String)
+24. perturb_ratio : Probability of agents taking action randomly. (Float)
+
+
+<br />
+
+In the "function_to_use" parameter above, below is the explanation for what these different values mean inside the list specified above.
+
+1. perturbed_response1: Agents select the best response (1-perturb_ratio)*100% times among the strategies which are most frequently used. If there is more than one such strategy, then agents select any one strategy randomly. Agents select random strategy (perturb_ratio)*100% times among the strategies which are not most frequently used. Here also, if there is more than one such strategy, then agents select any one strategy randomly out of these.
+2. perturbed_response2: Agent selects strategy randomly according to the relative weightage of different strategies. These relative weights are the % of times the respective strategy has been used by opponents in the past. 
+3. perturbed_response3: This is same as "perturbed_response1" function except agent selects random strategy (perturb_ratio)*100% times from all the possible strategies and not only from the ones which were not used most frequently by their opponents.
+4. perturbed_response4: Agent selects the best response 100% of times among the strategies which are most frequently used. If there is more than one such strategy, then agents select any one strategy randomly. There is no perturbation element (perturb_ratio is considered as zero).
+
+
+<br/>
+
+In the "network_name" parameter above, below is the explanation for what these different values mean inside the list specified above.
+1. small_world1: Returns a Watts Strogatz small-world graph. Here number of edges remained constant once we increase the prob_edge_rewire value. Shortcut edges if added would replace the existing ones. But total count of edges remained constant.
+2. small_world2: Returns a Newman Watts Strogatz small-world graph. Here number of edges increased once we increase the prob_edge_rewire value. It would add more shortcut edges in addition to what already exist.
+3. small_world3: Returns a connected Watts Strogatz small-world graph. Rest of the explanation remains as small_world1.
+4. complete: Returns the complete graph.
+5. random: Compute a random graph by swapping edges of a given graph. The given graph used is Watts Strogatz small-world graph (the one produced by "small_world1").
+6. grid2d: Return the 2d grid graph of mxn nodes, each connected to its nearest neighbors.
+
+We have used the networkx python library to populate these graphs. For more information around these graphs and how these are produced please refer to the link in the reference section.
+
+
+
+## Function explanation
+Here we explain the underlying functioning of this library with the help of an example. But this can be replicated to any symmetric game wherein we have defined finite strategies along with its payoff values.
+
+We assume there is a Nash demand game wherein each agent can make 3 demands, High (70), Medium (50) or Low (30). The rule of the game is if the total demands made by two agents in any given iteration are more than 100, no one is going to get anything. Below is the payoff matrix of row versus column player looks like.
+
+		  H	  M	    L
+    H	(0,0)	(0,0)	 (70,30)
+    M	(0,0)	(50,50)	 (50,30)
+    L	(30,70)	(30,50)	 (30,30)
+	
+
+There are 3 pure strategy Nash equilibria, (H, L), (M, M) and (L, H). There is not a strictly or weakly dominant strategy for any of the row or column player. Suppose that agents are connected in a ring network wherein each agent is connected with two other agents, one on the left and one on the right like in below image.
+
+
+![](https://github.com/ankur-tutlani/multi-agent-decision/raw/main/network_graph.png)
+
+
+Agents update their strategy if any of their neighbours (defined by "num_neighbors") are having higher payoff else, they stick to their own strategy which they have been following. Payoffs are computed as follows. If agent with strategy H meets agent with strategy M and L, then payoff from meeting with strategy M agent equals 0 and payoff from meeting with strategy L agent equals 70, hence the total payoff equals 70. In case of a tie, meaning payoffs are exactly same following current strategy versus payoffs from neighbours" strategy then agents stick to the strategy which they have been following. 
+
+We assume agents are distributed in a specific ratio in a network. E.g., if total agents ("num_agents") are 20 and if they are distributed in 40/40/20 distribution ("strategy_share"), that implies there are 8 H type agents, 8 M type agents and 4 L type agents. This can be represented in a list format like this [H,H,H,H,H,H,H,H,M,M,M,M,M,M,M,M,L,L,L,L]. This list shows first agent follows "H" (first value from the left), last agent follows "L" (last value from the right), agent 16 follows "M" etc.This list can be rearranged in multiple ways but still satisfies the condition of 40/40/20. Hence, we require to specify initial state of the agents in "agent_initial_state" parameter in the list format. If this parameter is empty, the function will select any one state randomly. This initial state is being shown in "initial_state_considered_..."  excel file output. For more details on the output generated, please refer to the section below.
+
+We start the game with one edge of the network is selected at any given point. Edge of the network is represented as (0,1), (5,4) etc, implying agents 0 and 1 are connected with each other, agents 5 and 4 are connected with each other. During each time period, all edges are selected sequentially and the agents associated with those edges play the game. We are interested in knowing how the initial state of H/M/L distribution changes as agents interact over a period of time and update their strategy. And how these results change when agents start the game with different initial states (e.g. more H type agents placed with H types or more H type agents placed with M type etc.).
+
+We have considered different combinations of strategies that agents can adopt while taking actions. We assume that agents use perturbed best response implying agents can take action randomly out of H,M or L with a certain positive probability (Young, 2015). At each time when agents require to take action, they look at the strategies of their neighbours and calculate their payoff. All agents calculate their payoffs in the current period and decide if they want to change strategies or stick to what they have been following so far. We have tested four different ways which agents can use to decide what action to take. The "function_to_use" parameter provides details about these and how these are different to each other.
+
+When the simulations are run for "num_of_trials" timeperiod, we get the percentage distribution of  H/M/L which agents used. This shows the percentage of agents who used H/M or L during each time period. The strategy which satisfy the two conditions for norm specified by "norms_agents_frequency" and "norms_time_frequency" are considered as norm. We have looked at two dimensions of norms, number of agents following the norm and for how long it has been followed. We can see the output like below. In below graph, X-axis shows the timeperiod, and Y-axis shows the % of agents who played the respective strategy. Y-axis values are in ratio format (range from 0 - 1), so would need to multiply by 100 to get this in percentage format. 
+
+
+![](https://github.com/ankur-tutlani/multi-agent-decision/raw/main/norm_emergence.png)
+
+
+
+In above figure, strategy "M" satisfies the norm criteria, when we assume "norms_agents_frequency" as 0.7 and "norms_time_frequency" as 0.5. This implies at least 70% of agents following "M" for at least 50% of times. The detailed explanation of the output generated is provided in the next section.
+
+We have also considered the possibility of norm displacement. This is controlled by three parameters, "enable_delta_payoff", "delta_to_add", and "min_time_period" parameters. For norm displacement, we need to specify "enable_delta_payoff" value to "Yes" and also specify a positive/negative value for "delta_to_add" parameter. The "min_time_period" parameter specifies the minimum time period for which the game should run before checking for norm displacement. Its value should be set lower than "num_of_trials" parameter. When any strategy satisfies the norm criteria laid out (say "M"), then the "delta_to_add" value is being added to the payoff values for rest of the other strategies ("H" and "L") after "min_time_period". The revised payoff matrix would be used by agents once the delta value is added to the payoff values. This would continue as long as some other strategy satisfies the norm criteria and the game is still not played for "num_of_trials" timeperiods. If some other strategy now satisfies the norm criteria (say "H"), then the delta payoff value would be added to the rest of the strategies ("M" and "L"). And this process continues till the game is played for all the timeperiods ("num_of_trials"). This can be seen in below figure where "M" strategy is being displaced by "H" strategy after around 40 timeperiods. And then again there is an attempt to displace "H" strategy with "M" strategy later in the game at around 90th timeperiod.
+
+
+![](https://github.com/ankur-tutlani/multi-agent-decision/raw/main/norm_displacement.png)
+
+
+
+## How to interpret output?
+There are total 10 files generated in the output when there is at least 1 strategy which satisfies the norm criteria.
+
+    input_network_ringnetwork_2023-02-02-21-31-34.png
+    networkgraph_initial_state_ringnetwork_2023-02-02-21-31-34.png
+    strategy_trend_ringnetwork_2023-02-02-21-31-34.png
+	network_after_100_timeperiods_ringnetwork_2023-02-02-21-31-34.png
+    normcandidates_ringnetwork_2023-02-02-21-31-34.xlsx
+    time_when_reached_norm_ringnetwork_2023-02-02-21-31-34.xlsx
+	parameters_ringnetwork_2023-02-02-21-31-34.xlsx
+	aggregate_data_detailed_agent_ringnetwork_2023-02-02-21-31-34.xlsx
+    initial_state_considered_ringnetwork_2023-02-02-21-31-34.xlsx
+	payoff_matrices_considered_by_timeperiod_ringnetwork_2023-02-02-21-31-34.xlsx
+    
+
+
+The 4 image files (.png) contain the network graphs and trend graph which is being considered for the simulation. The "input_network_.." file is the input network with which the game is started. "networkgraph_initial_state_...." file shows initial strategy distribution in the ratio specified in "strategy_share" parameter. The "strategy_trend_..." file shows the percent of agents following "H","M" or "L" strategy at each time period during the game. The "network_after_..." file is the network state at the end of game. Agents following the same strategy would be coloured in the same colour in this file.
+
+Norm file "normcandidates_..." shows strategy that satisfies the norm criteria laid out. File "time_when_reached_norm_..." shows the time period number when the specific strategy met the norm criteria. These 2 files are generated only when at least one strategy satisfies the norm criteria. 
+
+Parameters file "parameters_.." lists all the parameters which have been specified in the function call. File "aggregate_data_detailed_.." has the information on percentage of agents who proposed different strategies at each time period during the game. "initial_state_considered_" file shows the initial state with which game is started. In case of norm displacement, "payoff_matrices_considered_.." shows the payoff matrix considered along with time period. When there is more than one row in this file, this shows payoff matrix is being revised during the simulation run. The timeperiod column in this file shows the time period point at which the payoff matrix is revised.
+
+All the file names end with date and time stamp when the function was executed. It also contains information on network structure used like "ringnetwork" or "smallworld" network etc.
+
+
+## References
+1. Young, H.P. "The evolution of social norms" Annual Review of Economics. 2015 (7),pp.359-387
+2. https://pypi.org/project/networkx/ 
+
```

### Comparing `multi-agent-decision-0.2/setup.py` & `multi-agent-decision-0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,35 +4,35 @@
 def read_file(filename):
     with open(os.path.join(os.path.dirname(__file__), filename)) as file:
         return file.read()
 
 setup(
   name = 'multi-agent-decision',         
   packages = ['multi_agent_decision'],   
-  version = '0.2',      
+  version = '0.3',      
   license='MIT',        
   description = 'Simulates the actions which agents take under multi-agent systems and social networks',  
   long_description=read_file('README.md'),
   long_description_content_type='text/markdown',  
   author = 'ankurtutlani',                   
   author_email = 'ankur.tutlani@gmail.com',      
   url = 'https://github.com/ankur-tutlani/multi-agent-decision',   
-  download_url = 'https://github.com/ankur-tutlani/multi_agent_decision/archive/refs/tags/v_02.tar.gz',    
+  download_url = 'https://github.com/ankur-tutlani/multi_agent_decision/archive/refs/tags/v_03.tar.gz',    
   keywords = ['game theory', 'evolutionary game', 'social norms','multi-agent systems','evolution','social network','computational economics','simulation','agent-based modeling','computation'],   
   install_requires=[            
-          'numpy',
-		  'pandas',
-		  'networkx',
-		  'matplotlib',
-		  'setuptools'
+          'numpy>=1.24.3',
+		  'pandas>=2.0.3',
+		  'networkx>=3.1',
+		  'matplotlib>=3.7.2',
+		  'setuptools>=68.0.0'
 		  
 		  
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      
     'Intended Audience :: Developers',      
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   
 												
-	'Programming Language :: Python :: 3.7',
+	'Programming Language :: Python :: 3.11',
   ],
 )
```

