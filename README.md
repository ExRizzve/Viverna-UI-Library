<img width="627" height="511" alt="image" src="https://github.com/user-attachments/assets/d5b79844-9f76-4f7d-89a7-47e15fc492d8" />

Usage / Использование:

Start of the script - Начало скрипта

local VivUI = loadstring(game:HttpGet("https://raw.githubusercontent.com/ExRizzve/Viverna-UI-Library/main/VivUI.lua"))()

-- Creating a window / Создаем окно

local Window = VivUI.CreateWindow("your script", "")

-- Creating a tab / Создаем вкладку

local Tab = Window:Tab("Main", "")

-- Creating a section / Создаем секцию

local Section = Tab:Section("Features")

-- Adding elements / Добавляем элементы

Section:Button("click me", function()
    print("clicked")
end)

Section:Toggle("toggle", function(state)
    print(state)
end)

Section:Slider("speed", 0, 100, function(value)
    print(value)
end)
