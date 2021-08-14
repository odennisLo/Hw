# gRPC 的基本特色與四種傳輸說明與使用時機
* gRPC基本特色
 > gRPC 是針對低延遲和高輸送量的通訊所設計。 gRPC 非常適合於高效率的輕量微服務。
 > 點對點即時通訊： gRPC 有絕佳的雙向串流支援。gRPC services 可以即時推播訊息，而不會進行輪詢。
 > 網路受限的環境： gRPC 訊息會以 Protobuf （輕量訊息格式）進行序列化。 GRPC 訊息一律小於相等的 JSON 訊息。
 > 處理序間通訊 (ipc)：如 Unix 網域通訊端和具名管道等 ipc 傳輸，可與 gRPC 搭配使用，以在同一部電腦上的應用程式之間進行通訊。 如需詳細資訊，請參閱與 gRPC 的處理程序間通訊。
* gRPC四種傳輸說明和使用時機
1. 簡單模式 (simple)：類似傳統 API，client 發送 request 而 server 回傳 response,適用於一般API傳輸。
2. 服務端流式 (Server Streaming)：透過 HTTP/2，client 發送一次 request，而 server 可以回傳多次資料，適合從 server 端取得較大資料量時使用。
3. 客户端流式 (Client Streaming)：client 發送多次資料，直到告知 server 資料傳完後，server 再給予 response，適合傳送較大資料量至 server 端時使用。
4. 雙向數據流模式 (Bi Directional Streaming)：兩邊都用串流的方式傳送資料，適合在 client 與 server 端間雙向傳送大資料量或是即時資料時使用。



