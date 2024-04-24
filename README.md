makefolder("d_android_script_dir")

if _G.is_deltaandroid_loaded then
    print("already running")
    return
end

_G.is_deltaandroid_loaded = true

-- Instances: 310 | Scripts: 28 | Modules: 24
local G2L = {};

-- StarterGui.DeltaGui
G2L["1"] = Instance.new("ScreenGui", gethui());
G2L["1"]["Name"] = [[DeltaGui]];
G2L["1"]["ZIndexBehavior"] = Enum.ZIndexBehavior.Sibling;

-- StarterGui.DeltaGui.KeySystem
G2L["2"] = Instance.new("Folder", G2L["1"]);
G2L["2"]["Name"] = [[KeySystem]];

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame
G2L["3"] = Instance.new("Frame", G2L["2"]);
G2L["3"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
G2L["3"]["Size"] = UDim2.new(0.76389479637146, 0, 0.4519544541835785, 0);
G2L["3"]["Position"] = UDim2.new(0.11660274863243103, 0, 0.275360107421875, 0);
G2L["3"]["Visible"] = false;
G2L["3"]["Name"] = [[MainKeyFrame]];

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.SideFrame
G2L["4"] = Instance.new("Frame", G2L["3"]);
G2L["4"]["BackgroundColor3"] = Color3.fromRGB(0, 191, 255);
G2L["4"]["BackgroundTransparency"] = 1;
G2L["4"]["Size"] = UDim2.new(0.11645293235778809, 0, 1.0000001192092896, 0);
G2L["4"]["Name"] = [[SideFrame]];

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.SideFrame.Logo
G2L["5"] = Instance.new("ImageLabel", G2L["4"]);
G2L["5"]["BackgroundColor3"] = Color3.fromRGB(0, 191, 255);
G2L["5"]["Image"] = [[]];
G2L["5"]["Size"] = UDim2.new(1.0185703039169312, 0, 0.3629874587059021, 0);
G2L["5"]["Name"] = [[Logo]];
G2L["5"]["BackgroundTransparency"] = 1;
G2L["5"]["Position"] = UDim2.new(-0.018570121377706528, 0, 0.06093369424343109, 0);

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.SideFrame.Logo.UIAspectRatioConstraint
G2L["6"] = Instance.new("UIAspectRatioConstraint", G2L["5"]);
G2L["6"]["AspectRatio"] = 0.9946909546852112;

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.SideFrame.Frame
G2L["7"] = Instance.new("Frame", G2L["4"]);
G2L["7"]["BackgroundColor3"] = Color3.fromRGB(0, 191, 255);
G2L["7"]["Size"] = UDim2.new(0, 0, 0.9890000224113464, 0);
G2L["7"]["BorderColor3"] = Color3.fromRGB(0, 191, 255);
G2L["7"]["Position"] = UDim2.new(1, 0, 0.004999999888241291, 0);

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.SideFrame.Frame.UICorner
G2L["8"] = Instance.new("UICorner", G2L["7"]);
G2L["8"]["CornerRadius"] = UDim.new(0.09000000357627869, 0);

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.SideTextbox
G2L["9"] = Instance.new("Frame", G2L["3"]);
G2L["9"]["BackgroundColor3"] = Color3.fromRGB(0, 191, 255);
G2L["9"]["BackgroundTransparency"] = 0.33329999446868896;
G2L["9"]["Size"] = UDim2.new(0.8421385884284973, 0, 0.5559701919555664, 0);
G2L["9"]["BorderColor3"] = Color3.fromRGB(0, 191, 255);
G2L["9"]["Position"] = UDim2.new(0.13729187846183777, 0, 0.11194030940532684, 0);
G2L["9"]["Name"] = [[SideTextbox]];

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.SideTextbox.MainTextBox
G2L["a"] = Instance.new("TextBox", G2L["9"]);
G2L["a"]["TextSize"] = 13;
G2L["a"]["TextXAlignment"] = Enum.TextXAlignment.Left;
G2L["a"]["TextYAlignment"] = Enum.TextYAlignment.Top;
G2L["a"]["BackgroundColor3"] = Color3.fromRGB(0, 191, 255);
G2L["a"]["TextColor3"] = Color3.fromRGB(0, 191, 255);
G2L["a"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
G2L["a"]["BackgroundTransparency"] = 1;
G2L["a"]["PlaceholderText"] = [[Enter Your Key Here]];
G2L["a"]["Size"] = UDim2.new(0.9665210843086243, 0, 0.8322147727012634, 0);
G2L["a"]["BorderColor3"] = Color3.fromRGB(0, 191, 255);
G2L["a"]["Text"] = [[]];
G2L["a"]["Position"] = UDim2.new(0.020378457382321358, 0, 0.08053690940141678, 0);
G2L["a"]["Name"] = [[MainTextBox]];
G2L["a"]["ClearTextOnFocus"] = false;

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.SideTextbox.MainTextBox.UICorner
G2L["b"] = Instance.new("UICorner", G2L["a"]);
G2L["b"]["CornerRadius"] = UDim.new(0.09000000357627869, 0);

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.SideTextbox.UICorner
G2L["c"] = Instance.new("UICorner", G2L["9"]);
G2L["c"]["CornerRadius"] = UDim.new(0.09000000357627869, 0);

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.UICorner
G2L["d"] = Instance.new("UICorner", G2L["3"]);
G2L["d"]["CornerRadius"] = UDim.new(0.09000000357627869, 0);

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.UIAspectRatioConstraint
G2L["e"] = Instance.new("UIAspectRatioConstraint", G2L["3"]);
G2L["e"]["AspectRatio"] = 3.0439562797546387;

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.Continue
G2L["f"] = Instance.new("Frame", G2L["3"]);
G2L["f"]["BackgroundColor3"] = Color3.fromRGB(0, 191, 255)
G2L["f"]["Size"] = UDim2.new(0.19932664930820465, 0, 0.1760299652814865, 0);
G2L["f"]["Position"] = UDim2.new(0.13534526526927948, 0, 0.7490636706352234, 0);
G2L["f"]["Name"] = [[Continue]];

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.Continue.TextButton
G2L["10"] = Instance.new("TextButton", G2L["f"]);
G2L["10"]["TextWrapped"] = true;
G2L["10"]["TextScaled"] = true;
G2L["10"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0)
G2L["10"]["TextSize"] = 14;
G2L["10"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
G2L["10"]["TextColor3"] = Color3.fromRGB(0, 191, 255);
G2L["10"]["Size"] = UDim2.new(0.8136826753616333, 0, 1, 0);
G2L["10"]["Text"] = [[Continue]];
G2L["10"]["Position"] = UDim2.new(-0.004637444857507944, 0, 0, 0);

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.Continue.TextButton.UICorner
G2L["11"] = Instance.new("UICorner", G2L["10"]);
G2L["11"]["CornerRadius"] = UDim.new(0.4300000071525574, 0);

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.Continue.TextButton.LocalScript
G2L["12"] = Instance.new("LocalScript", G2L["10"]);


-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.Continue.TextButton.UITextSizeConstraint
G2L["13"] = Instance.new("UITextSizeConstraint", G2L["10"]);
G2L["13"]["MaxTextSize"] = 14;

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.Continue.UICorner
G2L["14"] = Instance.new("UICorner", G2L["f"]);
G2L["14"]["CornerRadius"] = UDim.new(0.4300000071525574, 0);

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.Continue.ImageLabel
G2L["15"] = Instance.new("ImageLabel", G2L["f"]);
G2L["15"]["BackgroundColor3"] = Color3.fromRGB(0, 191, 255);
G2L["15"]["Image"] = [[rbxassetid://12730588268]];
G2L["15"]["Size"] = UDim2.new(0.1541670262813568, 0, 0.5313842296600342, 0);
G2L["15"]["BackgroundTransparency"] = 1;
G2L["15"]["Position"] = UDim2.new(0.6577792763710022, 0, 0.2479792982339859, 0);

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.GetKey
G2L["16"] = Instance.new("Frame", G2L["3"]);
G2L["16"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0)
G2L["16"]["Size"] = UDim2.new(0.19932664930820465, 0, 0.1760299652814865, 0);
G2L["16"]["Position"] = UDim2.new(0.34697607159614563, 0, 0.7490636706352234, 0);
G2L["16"]["Name"] = [[GetKey]];

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.GetKey.TextButton
G2L["17"] = Instance.new("TextButton", G2L["16"]);
G2L["17"]["TextWrapped"] = true;
G2L["17"]["TextScaled"] = true;
G2L["17"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
G2L["17"]["TextSize"] = 14;
G2L["17"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
G2L["17"]["TextColor3"] = Color3.fromRGB(0, 191, 255);
G2L["17"]["Size"] = UDim2.new(0.8136826753616333, 0, 1, 0);
G2L["17"]["Text"] = [[Get Key]];
G2L["17"]["Position"] = UDim2.new(-0.004637444857507944, 0, 0, 0);

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.GetKey.TextButton.UICorner
G2L["18"] = Instance.new("UICorner", G2L["17"]);
G2L["18"]["CornerRadius"] = UDim.new(0.4300000071525574, 0);

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.GetKey.TextButton.LocalScript
G2L["19"] = Instance.new("LocalScript", G2L["17"]);


-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.GetKey.TextButton.UITextSizeConstraint
G2L["1a"] = Instance.new("UITextSizeConstraint", G2L["17"]);
G2L["1a"]["MaxTextSize"] = 14;

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.GetKey.UICorner
G2L["1b"] = Instance.new("UICorner", G2L["16"]);
G2L["1b"]["CornerRadius"] = UDim.new(0.4300000071525574, 0);

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.GetKey.ImageLabel
G2L["1c"] = Instance.new("ImageLabel", G2L["16"]);
G2L["1c"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0)
G2L["1c"]["Image"] = [[rbxassetid://12730592157]];
G2L["1c"]["Size"] = UDim2.new(0.14388921856880188, 0, 0.4959585964679718, 0);
G2L["1c"]["BackgroundTransparency"] = 1;
G2L["1c"]["Position"] = UDim2.new(0.6577792763710022, 0, 0.2479792982339859, 0);

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.JoinServer
G2L["1d"] = Instance.new("Frame", G2L["3"]);
G2L["1d"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0)
G2L["1d"]["Size"] = UDim2.new(0.23844483494758606, 0, 0.1760299652814865, 0);
G2L["1d"]["Position"] = UDim2.new(0.5598372220993042, 0, 0.7490636706352234, 0);
G2L["1d"]["Name"] = [[JoinServer]];

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.JoinServer.TextButton
G2L["1e"] = Instance.new("TextButton", G2L["1d"]);
G2L["1e"]["TextWrapped"] = true;
G2L["1e"]["TextScaled"] = true;
G2L["1e"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0)
G2L["1e"]["TextSize"] = 14;
G2L["1e"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
G2L["1e"]["TextColor3"] = Color3.fromRGB(0, 191, 255);
G2L["1e"]["Size"] = UDim2.new(0.8136826753616333, 0, 1, 0);
G2L["1e"]["Text"] = [[ENTRE DISCORD]];
G2L["1e"]["Position"] = UDim2.new(-0.004637444857507944, 0, 0, 0);

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.JoinServer.TextButton.UICorner
G2L["1f"] = Instance.new("UICorner", G2L["1e"]);
G2L["1f"]["CornerRadius"] = UDim.new(0.4300000071525574, 0);

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.JoinServer.TextButton.LocalScript
G2L["20"] = Instance.new("LocalScript", G2L["1e"]);


-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.JoinServer.TextButton.UITextSizeConstraint
G2L["21"] = Instance.new("UITextSizeConstraint", G2L["1e"]);
G2L["21"]["MaxTextSize"] = 14;

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.JoinServer.UICorner
G2L["22"] = Instance.new("UICorner", G2L["1d"]);
G2L["22"]["CornerRadius"] = UDim.new(0.4300000071525574, 0);

-- StarterGui.DeltaGui.KeySystem.MainKeyFrame.JoinServer.ImageLabel
G2L["23"] = Instance.new("ImageLabel", G2L["1d"]);
G2L["23"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
G2L["23"]["Image"] = [[rbxassetid://12730595164]];
G2L["23"]["Size"] = UDim2.new(0.11047418415546417, 0, 0.4959585964679718, 0);
G2L["23"]["BackgroundTransparency"] = 1;
G2L["23"]["Position"] = UDim2.new(0.6944091320037842, 0, 0.2479792982339859, 0);

-- StarterGui.DeltaGui.MainUi
G2L["24"] = Instance.new("Folder", G2L["1"]);
G2L["24"]["Name"] = [[MainUi]];

-- StarterGui.DeltaGui.MainUi.MainFrame
G2L["25"] = Instance.new("Frame", G2L["24"]);
G2L["25"]["Active"] = true;
G2L["25"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
G2L["25"]["Size"] = UDim2.new(0.6537454724311829, 0, 0.9718542695045471, 0);
G2L["25"]["Position"] = UDim2.new(0.17294080555438995, 0, 0.013245033100247383, 0);
G2L["25"]["Visible"] = true;
G2L["25"]["Name"] = [[MainFrame]];

-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame
G2L["26"] = Instance.new("Frame", G2L["25"]);
G2L["26"]["BackgroundColor3"] = Color3.fromRGB(0, 191, 255);
G2L["26"]["BackgroundTransparency"] = 1;
G2L["26"]["Size"] = UDim2.new(0.11645293235778809, 0, 1.0000001192092896, 0);
G2L["26"]["Name"] = [[SideFrame]];

-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Logo
G2L["27"] = Instance.new("ImageLabel", G2L["26"]);
G2L["27"]["BackgroundColor3"] = Color3.fromRGB(0, 191, 255);
G2L["27"]["Image"] = [[rbxassetid://5261175692]];
G2L["27"]["Size"] = UDim2.new(1.0080041885375977, 0, 0.1372550129890442, 0);
G2L["27"]["Name"] = [[Logo]];
G2L["27"]["BackgroundTransparency"] = 1;
G2L["27"]["Position"] = UDim2.new(0.013000000268220901, 0, 0.022535257041454315, 0);

-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Logo.UIAspectRatioConstraint
G2L["28"] = Instance.new("UIAspectRatioConstraint", G2L["27"]);


-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Frame
G2L["29"] = Instance.new("Frame", G2L["26"]);
G2L["29"]["BackgroundColor3"] = Color3.fromRGB(0, 191, 255);
G2L["29"]["Size"] = UDim2.new(0, 0, 0.9890000224113464, 0);
G2L["29"]["BorderColor3"] = Color3.fromRGB(0, 191, 255);
G2L["29"]["Position"] = UDim2.new(1, 0, 0.004999999888241291, 0);

-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Frame.UICorner
G2L["2a"] = Instance.new("UICorner", G2L["29"]);
G2L["2a"]["CornerRadius"] = UDim.new(0.09000000357627869, 0);

-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Buttons
G2L["2b"] = Instance.new("Folder", G2L["26"]);
G2L["2b"]["Name"] = [[Buttons]];

-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Buttons.Home
G2L["2c"] = Instance.new("ImageButton", G2L["2b"]);
G2L["2c"]["BackgroundColor3"] = Color3.fromRGB(0, 191, 255);
G2L["2c"]["Image"] = [[rbxassetid://12731028861]];
G2L["2c"]["Size"] = UDim2.new(0.5177212357521057, 0, 0.08347529172897339, 0);
G2L["2c"]["Name"] = [[Home]];
G2L["2c"]["Position"] = UDim2.new(0.2218806892633438, 0, 0.29020607471466064, 0);
G2L["2c"]["BackgroundTransparency"] = 1;

-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Buttons.Home.UIAspectRatioConstraint
G2L["2d"] = Instance.new("UIAspectRatioConstraint", G2L["2c"]);


-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Buttons.Home.OffImage
G2L["2e"] = Instance.new("StringValue", G2L["2c"]);
G2L["2e"]["Value"] = [[rbxassetid://12731028861]];
G2L["2e"]["Name"] = [[OffImage]];

-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Buttons.Home.OnImage
G2L["2f"] = Instance.new("StringValue", G2L["2c"]);
G2L["2f"]["Value"] = [[rbxassetid://12731052548]];
G2L["2f"]["Name"] = [[OnImage]];

-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Buttons.Home.LocalScript
G2L["30"] = Instance.new("LocalScript", G2L["2c"]);


-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Buttons.MakeScript
G2L["31"] = Instance.new("ImageButton", G2L["2b"]);
G2L["31"]["BackgroundColor3"] = Color3.fromRGB(0, 191, 255);
G2L["31"]["Image"] = [[rbxassetid://12730930487]];
G2L["31"]["Size"] = UDim2.new(0.5177212357521057, 0, 0.08347529172897339, 0);
G2L["31"]["Name"] = [[MakeScript]];
G2L["31"]["Position"] = UDim2.new(0.2424367517232895, 0, 0.186909481883049, 0);
G2L["31"]["BackgroundTransparency"] = 1;

-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Buttons.MakeScript.UIAspectRatioConstraint
G2L["32"] = Instance.new("UIAspectRatioConstraint", G2L["31"]);


-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Buttons.MakeScript.OffImage
G2L["33"] = Instance.new("StringValue", G2L["31"]);
G2L["33"]["Value"] = [[rbxassetid://12730888709]];
G2L["33"]["Name"] = [[OffImage]];

-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Buttons.MakeScript.OnImage
G2L["34"] = Instance.new("StringValue", G2L["31"]);
G2L["34"]["Value"] = [[rbxassetid://12730930487]];
G2L["34"]["Name"] = [[OnImage]];

-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Buttons.MakeScript.LocalScript
G2L["35"] = Instance.new("LocalScript", G2L["31"]);


-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Buttons.Minimize
G2L["36"] = Instance.new("ImageButton", G2L["2b"]);
G2L["36"]["BackgroundColor3"] = Color3.fromRGB(0, 191, 255);
G2L["36"]["Image"] = [[rbxassetid://12731990314]];
G2L["36"]["Size"] = UDim2.new(0.5177212357521057, 0, 0.08347529172897339, 0);
G2L["36"]["Name"] = [[Minimize]];
G2L["36"]["Position"] = UDim2.new(0.2218806892633438, 0, 0.8980652093887329, 0);
G2L["36"]["BackgroundTransparency"] = 1;

-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Buttons.Minimize.UIAspectRatioConstraint
G2L["37"] = Instance.new("UIAspectRatioConstraint", G2L["36"]);


-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Buttons.Minimize.OffImage
G2L["38"] = Instance.new("StringValue", G2L["36"]);
G2L["38"]["Value"] = [[rbxassetid://12731990314]];
G2L["38"]["Name"] = [[OffImage]];

-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Buttons.Minimize.OnImage
G2L["39"] = Instance.new("StringValue", G2L["36"]);
G2L["39"]["Value"] = [[rbxassetid://12731990314]];
G2L["39"]["Name"] = [[OnImage]];

-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Buttons.Minimize.LocalScript
G2L["3a"] = Instance.new("LocalScript", G2L["36"]);


-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Buttons.Settings
G2L["3b"] = Instance.new("ImageButton", G2L["2b"]);
G2L["3b"]["BackgroundColor3"] = Color3.fromRGB(0, 191, 255);
G2L["3b"]["Image"] = [[rbxassetid://12731105925]];
G2L["3b"]["Size"] = UDim2.new(0.5177212357521057, 0, 0.08347529172897339, 0);
G2L["3b"]["Name"] = [[Settings]];
G2L["3b"]["Position"] = UDim2.new(0.2424367517232895, 0, 0.5168625116348267, 0);
G2L["3b"]["BackgroundTransparency"] = 1;

-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Buttons.Settings.UIAspectRatioConstraint
G2L["3c"] = Instance.new("UIAspectRatioConstraint", G2L["3b"]);


-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Buttons.Settings.OffImage
G2L["3d"] = Instance.new("StringValue", G2L["3b"]);
G2L["3d"]["Value"] = [[rbxassetid://12731105925]];
G2L["3d"]["Name"] = [[OffImage]];

-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Buttons.Settings.OnImage
G2L["3e"] = Instance.new("StringValue", G2L["3b"]);
G2L["3e"]["Value"] = [[rbxassetid://12731109653]];
G2L["3e"]["Name"] = [[OnImage]];

-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Buttons.Settings.LocalScript
G2L["3f"] = Instance.new("LocalScript", G2L["3b"]);


-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Buttons.Scripts
G2L["40"] = Instance.new("ImageButton", G2L["2b"]);
G2L["40"]["BackgroundColor3"] = Color3.fromRGB(0, 191, 255);
G2L["40"]["Image"] = [[rbxassetid://12731084214]];
G2L["40"]["Size"] = UDim2.new(0.5177212357521057, 0, 0.08347529172897339, 0);
G2L["40"]["Name"] = [[Scripts]];
G2L["40"]["Position"] = UDim2.new(0.2218806892633438, 0, 0.40612998604774475, 0);
G2L["40"]["BackgroundTransparency"] = 1;

-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Buttons.Scripts.UIAspectRatioConstraint
G2L["41"] = Instance.new("UIAspectRatioConstraint", G2L["40"]);


-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Buttons.Scripts.OffImage
G2L["42"] = Instance.new("StringValue", G2L["40"]);
G2L["42"]["Value"] = [[rbxassetid://12731084214]];
G2L["42"]["Name"] = [[OffImage]];

-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Buttons.Scripts.OnImage
G2L["43"] = Instance.new("StringValue", G2L["40"]);
G2L["43"]["Value"] = [[rbxassetid://12731089712]];
G2L["43"]["Name"] = [[OnImage]];

-- StarterGui.DeltaGui.MainUi.MainFrame.SideFrame.Buttons.Scripts.LocalScript
G2L["44"] = Instance.new("LocalScript", G2L["40"]);


-- StarterGui.DeltaGui.MainUi.MainFrame.UICorner
G2L["45"] = Instance.new("UICorner", G2L["25"]);
G2L["45"]["CornerRadius"] = UDim.new(0.03999999910593033, 0);

-- StarterGui.DeltaGui.MainUi.MainFrame.Tabs
G2L["46"] = Instance.new("Folder", G2L["25"]);
G2L["46"]["Name"] = [[Tabs]];

-- StarterGui.DeltaGui.MainUi.MainFrame.Tabs.MakeScript
G2L["47"] = Instance.new("Frame", G2L["46"]);
G2L["47"]["BackgroundColor3"] = Color3.fromRGB(0, 191, 255);
G2L["47"]["BackgroundTransparency"] = 1;
G2L["47"]["Size"] = UDim2.new(0.8833174705505371, 0, 0.9945666193962097, 0);
G2L["47"]["Position"] = UDim2.new(0.11490308493375778, 0, 0.002866186201572418, 0);
G2L["47"]["Name"] = [[MakeScript]];

-- StarterGui.DeltaGui.MainUi.MainFrame.Tabs.MakeScript.TitleScript
G2L["48"] = Instance.new("Frame", G2L["47"]);
G2L["48"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
G2L["48"]["BackgroundTransparency"] = 0.33329999446868896;
G2L["48"]["Size"] = UDim2.new(0.9585282802581787, 0, 0.0768190324306488, 0);
G2L["48"]["BorderColor3"] = Color3.fromRGB(0, 191, 255);
G2L["48"]["Position"] = UDim2.new(0.0236122515052557, 0, 0.019721297547221184, 0);
G2L["48"]["Visible"] = false;
G2L["48"]["Name"] = [[TitleScript]];

-- StarterGui.DeltaGui.MainUi.MainFrame.Tabs.MakeScript.TitleScript.MainTextBox
G2L["49"] = Instance.new("TextBox", G2L["48"]);
G2L["49"]["PlaceholderColor3"] = Color3.fromRGB(0, 191, 255);
G2L["49"]["TextSize"] = 13;
G2L["49"]["TextXAl
