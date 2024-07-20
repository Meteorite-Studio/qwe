## Page System Project

> [!NOTE]
> This project is stil on beta.
#
> [!IMPORTANT]
> Requiring Project
> ```lua
> --// Code Language: LUA
> --// OBJECT TYPE AVAILABILITY: SCRIPT
> require(18575752996):Load()
> ```
#
> [!IMPORTANT]
> Changing Automatic Limit Page / function :SetAutomaticLimitPageTo() -- Automatic limit page will automatically set the limit of the page depending how many page it contains
> ```lua
> --// Code Language: LUA
> --// OBJECT TYPE AVAILABILITY: localscript
> local PageSystem = game.ReplicatedStorage:WaitForChild("PageSystem")
>
> PageSystem:SetAutomaticLimitPageTo(Boolean : boolean) -- true/false
> ```
#
> [!IMPORTANT]
> Changing Prefix to look for / function :SetPagePrefixNameTo -- Look for the frame that has a same name as the prefix for e.g "Page..CurrentPage" or "Page1" numbers is neccesary so it indicate the where is the next page.
> ```lua
> --// Code Language: LUA
> --// OBJECT TYPE AVAILABILITY: localscript
> local PageSystem = game.ReplicatedStorage:WaitForChild("PageSystem")
>
> PageSystem:SetPagePrefixNameTo(Name : string) -- string
> ```
#
> [!IMPORTANT]
> Next Page / function .Next -- Proceed to next page. Make sure the page are inside the Pages folder and set it to P1 (Default Prefix)
> 
> ![image](https://github.com/user-attachments/assets/574929b4-0ee6-44e5-a53d-dbc05ccf7e89)
> ```lua
> --// Code Language: LUA
> --// OBJECT TYPE AVAILABILITY: localscript
> local PageSystem = game.ReplicatedStorage:WaitForChild("PageSystem")
>
> PageSystem.Next(Pages : Folder?) -- Object
> ```
#
> [!IMPORTANT]
> Previous Page / function .Previous -- Go back to previous page. Make sure the page are inside the Pages folder and set it to P1 (Default Prefix)
> 
> ![image](https://github.com/user-attachments/assets/574929b4-0ee6-44e5-a53d-dbc05ccf7e89)
> ```lua
> --// Code Language: LUA
> --// OBJECT TYPE AVAILABILITY: localscript
> local PageSystem = game.ReplicatedStorage:WaitForChild("PageSystem")
>
> PageSystem.Previous(Pages: Folder?) -- Object
> ```
#
> [!IMPORTANT]
> Update / function .Update -- Update the page. This function should be keep repeating, so the next and previous button will be controlled
> ```lua
> --// Code Language: LUA
> --// OBJECT TYPE AVAILABILITY: localscript
> local PageSystem = game.ReplicatedStorage:WaitForChild("PageSystem")
>
> while wait(0.5) do
>   PageSystem.Update(Pages : Folder,Previous : Button, Next: Button) -- Object, Object, Object
> end)
> ```
#
> [!TIP]
> Here is the example
>
> You can use this as a guide to follow (The prefix used is "P" which is the default one, to add a new page just change the number after the prefix but make sure all of it was following the increasing rules or else it will not work)
> 
> ![image](https://github.com/user-attachments/assets/5804033b-ee07-4f2e-8d47-fc3a376eb5d7)
>
> The script inside it:
>
> ![image](https://github.com/user-attachments/assets/be9c19ef-aed8-439a-9e61-591feadf6c05)


