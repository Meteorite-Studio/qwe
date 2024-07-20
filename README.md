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
> Changing Automatic Limit Page / function :SetAutomaticLimitPageTo() -- The automatic limit page will set the page limit based on the total number of pages.
> ```lua
> --// Code Language: LUA
> --// OBJECT TYPE AVAILABILITY: localscript
> local PageSystem = game.ReplicatedStorage:WaitForChild("PageSystem")
>
> PageSystem:SetAutomaticLimitPageTo(Boolean : boolean) -- true/false
> ```
#
> [!IMPORTANT]
> Changing Prefix to look for / function :SetPagePrefixNameTo -- Find the frame that matches the prefix, such as "Page..CurrentPage" or "Page1." Numbers are necessary as they indicate the order of the pages.
> ```lua
> --// Code Language: LUA
> --// OBJECT TYPE AVAILABILITY: localscript
> local PageSystem = game.ReplicatedStorage:WaitForChild("PageSystem")
>
> PageSystem:SetPagePrefixNameTo(Name : string) -- string
> ```
#
> [!IMPORTANT]
> Next Page / function .Next -- Proceed to the next page. Ensure the page is inside the Pages folder and set the name to P1 (Default Prefix).
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
> Previous Page / function .Previous -- Go back to the previous page. Ensure the page is inside the Pages folder and set the name to P1 (Default Prefix).
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
> Update / function .Update -- Update the page. This function should keep repeating, so the next and previous buttons will be controlled.
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
> You can use this as a guide to follow: The prefix used is "P" (the default). To add a new page, just change the number after the prefix, ensuring all numbers follow the increasing sequence; otherwise, it will not work.
> 
> ![image](https://github.com/user-attachments/assets/5804033b-ee07-4f2e-8d47-fc3a376eb5d7)
>
> The script inside it:
>
> ![image](https://github.com/user-attachments/assets/be9c19ef-aed8-439a-9e61-591feadf6c05)


