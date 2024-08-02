## **Latest release: https://github.com/Maebbie/Udon-Graph-Triggers/releases**

**Udon Graph Triggers** contains an essential assortment of Triggers ready to use for setting up basic world interactions.
These behaviours run entirely on vanilla Udon Graph and require no UdonSharp and no other dependencies to work. They exist to remove dependency of 3. parties to continue maintaining their projects.
Simple triggers should only need simple requirements.

<img src="https://github.com/user-attachments/assets/6a05e8db-eacf-444a-9332-e670c2ac3c3f" width="640">

Found here are over 50 separate single purpose behaviours, that are loosely based on the old SDK2 trigger system's functionality. Nodes are set at the same position on the graph across all behaviours found here. This means Events, SetActive and other nodes that occur multiple times are always found at the same spot.

To use these, simply add a Udon Behaviour Script to a Game Object and drag the desired Behaviour into the "Program Source" field. All relevant options appear afterwards.

Naming Convention is as follows:\
```Event Type - Affecting - State```

For example:\
```OnInteract - GameObject - Toggle``` -> OnInteract-GameObject-Toggle.asset\
```OnEnable   - GameObject - On    ``` -> OnEnable-GameObject-On.asset

| Event |  |
| :--- | :--- |
|On Enable | As soon as the Object is enabled, often used to activate on World being loaded.|
|On Enter Station | When entering a Seat|
|On Exit Station | When leaving a Seat|
|On Interact | When interacting with a button or similar|
|On Player Enter Trigger | When entering a trigger area|
|On Player Exit Trigger | When exiting a trigger area|
|On Player joined | When a Player joins|
|On local Player joined | When you join and successfully connect|

| Affecting |  |
| :--- | :--- |
|GameObjects | "targets" can be multiple ones. A number of targets above 1 needs to be input to use more than 1.|
|AnimatorBool | target here is the GameObject that has the Animator component.|
|Collider | target here is the GameObject, it will select the collider automatically.|

| State |
| :--- |
|On|
|Off|
|Toggle|
|with delay|
|with a random chance to activate|

Requirements
Only the VRChat SDK

I developed these as part of my efforts to make maintaining my VRChat Worlds as easy as possible. Having to rely on anything other than the VRChat SDK and potentially replacing tools can be a time drain in the future that is easily avoidable.

~Maebbie
