local wezterm = require 'wezterm'

return {
  -- 基本外观
  font = wezterm.font("JetBrains Mono"),  -- 等宽编程字体
  font_size = 14.0,
  line_height = 1.2,
  color_scheme = "Catppuccin Mocha",      -- 推荐深色主题
  window_background_opacity = 0.95,       -- 轻微透明
  enable_tab_bar = true,                  -- 显示标签页
  -- 右下角显示当前工作区和时间
  status_update_interval = 1000,
  enable_wayland = false,  -- Linux 可根据需要改
  keys = {
    {
      key = "h",
      mods = "CTRL|SHIFT",
      action = wezterm.action.SplitHorizontal { domain = "CurrentPaneDomain" },
    },
    {
      key = "v",
      mods = "CTRL|SHIFT",
      action = wezterm.action.SplitVertical { domain = "CurrentPaneDomain" },
    },
    {
      key = "c",
      mods = "CTRL|SHIFT",
      action = wezterm.action.CopyTo("Clipboard"),
    },
    {
      key = "v",
      mods = "CTRL",
      action = wezterm.action.PasteFrom("Clipboard"),
    },
  },

  ssh_domains = {
    {
      name = 'turing-web-ide',
      remote_address = '127.0.0.1',
      username = 'developer',
      multiplexing = "WezTerm",
    },
  },
}