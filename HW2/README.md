# 請說明.NET Core .NET Standard 與 .NET Framework的差別與優略
* .NET Core 
  差異:
  1. .NET Core 是 .NET 的最新實現，可在 Windows、Linux 和 macOS 上運行
  2. 其開源和微軟接受第三方對 .NET Core 的貢獻
  3. 它支持 3.0 版的桌面框架，如 Windows Forms 和 WPF
  優點:
  1. 支援跨平台需求
  2. 適合使用Docker等容器技術
  3. 需要高效能、可延展 的應用系統
  4. 可以並存不同的 NET 版本 降低相依性
* .NET Framework
  差異:
  1. .NET Framework 是第一個僅適用於 Windows 的 .NET 實現
  2. 它的源代碼是公開的，但微軟不接受第三方的貢獻
  優點:
  1. 大量第三方函式庫或套件
  2. 穩定的版本
* .NET Standard
  差異：
  1. .NET Standard 是一種規範，而不是 .NET 實現
  2. 它指定了所有 .NET 實現都必須實現的一組 API
  3. 我們只能用它創建類庫類型的項目
  優點:
  1. 定義一個標準介面讓你可以透過此標準介面在不同平台下皆可使用一致的BCL資源