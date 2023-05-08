[Speckle](https://speckle.systems/tutorials/unreal-engine-blueprint-nodes-fetch-stream-branch-commit-info-and-more/) seems like a very good connector option
	For [grasshopper](https://speckle.guide/user/grasshopper.html)
[Speckle repository](https://github.com/specklesystems/speckle-unreal)
This [person](https://github.com/JR-Morgan) from the Speckle team might have some insights into how to build with Speckle for VR/AR [1](https://speckle.community/t/unity-android-build/3104/7), [2](https://speckle.community/t/virtual-augmented-reality/4467), [3](https://speckle.community/t/receiving-speckle-streams-in-ios-apps/1910/5)

- For now I will follow [this tutorial](https://www.youtube.com/watch?v=O45ZY9H7gx4): this tutorial for [grashopper](https://speckle.systems/tutorials/getting-started-with-speckle-for-grasshopper/) and this one [for installing](https://www.youtube.com/watch?v=vb2yL5qLql8&t=31s)
	- Using architecture blank project as template
		- ![Pasted image 20230503120122](../media/Pasted%20image%2020230503120122.png)
	- Enabling the plugin from Edit/Plugins...search for Speckle
	- Create a token in my Speckle profile: `6b13930da22e4d2b3360dbaa754db7f83553fbf50b`
	- Open place actor sidebar using Window -> PlaceActor
		- Added the info of my token 
	- Create the Stream in Speckle.
		- Install the Manager for Speckle
		- Install the Grashopper conntection there which installs Speckle in Grasshopper
		- Send the data to the stream service
		- This is the stream I am working with: https://speckle.xyz/streams/992b7b3e37/commits/a56bb91748?c=%5B0.03292,-0.01013,0.02259,-0.00641,0.00312,0.00329,1,0.6521738445200155%5D
		
		![Pasted image 20230503132948](../media/Pasted%20image%2020230503132948.png)
	- Sending objects to unreal
		- In grasshopper I have to create a [Speckle object](https://speckle.systems/tutorials/custom-speckle-object-strategies/) to group elements in a root object that I can access into the game engine id 
		- ![Pasted image 20230508101752](../media/Pasted%20image%2020230508101752.png)
	- Automatically sending:
		- ![Grashopper Sync](videos_exp_2_speckle/Grashopper%20Sync.gif)
		- [Apparently it is not yet supported in Unreal to automatically receive objects](https://github.com/specklesystems/speckle-unreal/issues/61) 
		- [Sending automatically works in grasshopper](https://speckle.community/t/automatic-update-in-grasshopper/2024)