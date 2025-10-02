### Part 1: Paxos & Raft exercise

We will be communicating only using paper when communicating with other teams to avoid information leaks. Do not speak loudly in own team when executing an algorithm. Only use pen and paper in these cases as well. 

Split in x teams of y people. x > 10, 2 < y < 5  Pick team names. 

#### Phase 1: Use your own means within your team (phone timers etc) to simulate a raft-based leader election and elect 1 of each : 1 leader, 1 team messenger, 1 teacher messenger

 - Teacher messenger of each team comes to communicate with teacher. 

#### Phase 2: You have the following options (burgers, pizza, kebab, McDonnalds). Together pick a version of the reliable consensus algorithm (slide 6, 9,19) depending on what you think is best. Purpose is to agree on what your team would like to eat. 

 - We wrap up phase 2. Leaders of teams allowed to discuss with whole classroom. 

#### Phase 3: Again: use only paper when communicating with other teams. Our university has sent us to a giant CS conference and the teams we have formed had different presentations at different times. We would like to go eat together all the AAU people. Some teams might drop out because they were invited by people in the same session as them to go out. 

 - Use paxos to start communicating with other teams. On your papers write your current message content, team names, and ID and anything else paxos requires. Send your messenger and wait for them to get back with the response from other team. Do this at the speed you can. 

 - Sent your teacher messenger once you are sure you have found the agreed value on food. 

#### Phase 4: Okay we sit down again and discuss. How big was a quorum today? Any intuition why? 


----------------------------------------------------------------------------------------------------------------


Given a Total order broadcast algorithm design a consensus protocol. Also do the opposite. 

Give an example with n = 5 and f = 1 in the iterative byzantine generals probelm. Show that the algorithm reaches agreement. 

For the byzantine generals problem, show how to generalise with 2 rounds when f = 2. 

Write pseudocode for the PAXOS module.