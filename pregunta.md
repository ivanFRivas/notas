funciono foot -e sudo pacman -Syu, pero quiero hacer una pausa. primero estaba inicializando hyprland usando hyprland, aparecia una leyenda que sugeria start-hyprland en lu lugar, aparcio entonces con un fondo diferente, talvez fue casualidad, no se.  segundo, mi archivo de configuracion esta en lua, entonces quedo
 hl.on("hyprland.start", function () 
--   hl.exec_cmd(terminal)
--   hl.exec_cmd("nm-applet")
--   hl.exec_cmd("waybar & hyprpaper & firefox")
     hl.exec_cmd("systemctl --user start hyprpolkitagent")
 end)
