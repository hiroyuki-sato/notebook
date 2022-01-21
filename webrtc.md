##

### 4.2 [Configuration](https://www.w3.org/TR/webrtc/#configuration)

```yaml
iceServers:
# RTCIceServer
- urls: stun:stun1.example.net
- urls:
  - turns:turn.example.org
  - turn:turn.example.net
  uesrname: user
  credential: myPassword
  credentialType: password
iceTransportPolicy: relay
#iceTransportPolicy: all
bundlePolicy: balanced
#bundlePolicy: max-compat
#bundlePolicy: max-bundle
rtcpMuxPolicy: require
certificates:
- cert1 # TODO
- cert2 # TODO
- cert3 # TODO
```

### 4.3 [State Definitions](https://www.w3.org/TR/webrtc/#state-definitions)

#### 4.3.1 RTCSignalingState

* stable
* have-local-offer
* have-remote-offer
* have-local-pranswer
* have-remote-pranswer
* closed

#### 4.3.2 RTCIceGatheringState

* new
* gathering
* complete

#### 4.3.3 RTCPeerConnectionState 

* closed
* failed
* disconnected
* new
* connecting
* connected

#### 4.3.4 RTCIceConnectionState 

* closed
* failed
* disconnected
* new
* cheking
* completed
* connected

### 4.4  [RTCPeerConnection Interface](https://www.w3.org/TR/webrtc/#rtcpeerconnection-interface)

#### 4.4.1 Operation

* `new RTCPeerConnection(configuration)` で `RTCPeerConnection` オブジェクトを作る
* `configuration`にはiceServersの情報を渡すことができる
* `RTCPeerConnection` オブジェクトは次の状態を内部で持っている
  * signaling state
  * connection state
  * ICE gathering state
  * ICE connetion state
* `RTCPeerConnection` 内のICEプロトコルの実装はRFC 5245のICE Agentによって実現される
* ICE Agentと強調して動作するメソッド群
  * addIceCandidate
  * setConfiguration
  * setLocalDescription
  * setRemoteDescription
  * close
* ICE Agentは内部で、`RTCIceTransport` の状態を管理する
* SDPの注意書き後述

#### 4.4.1.1 コンストラクタ

1. 処理に失敗したら、エラーをおこす。
2. Let connection be a newly created RTCPeerConnection object. (Let .. be ..をそのままにしておく)
3. 
4.
5.
6.
7. ICE Agentの初期化
8. iceTransportPolicyが未定義だったら、allを
9. bundlePolicyがい定義だったら、balanced
10. rtcpMuxPolicyが未定義だったら、require
11. Configuration
12. IsClosed: false
13. NegotiationNeeded: false
14. SctpTransport: null
15. Operations: 空
16. UpdateNegotiationNeededFlagOnEmptyChain: false
17. LastCreatedOffer: ""
18. LastCreatedAnswer: ""
19. EarlyCandidates: 空リスト
20. 状態 signaling: stable
21. 状態 iceConnectionState: new
22. 状態 iceGatheringState: new
23. 状態 connection: new
24. PendingLocalDescription: 空
25. CurrentLocalDescription: 空
26. PendingRemoteDescription: 空
27. CurrentRemoteDescription: 空
28. LocalIceCredentialsToReplace: 空
29. connectionを返す

#### 4.4.1.2 Chain an asynchronous operation
#### 4.4.1.3 Update the connection state
#### 4.4.1.4 Update the ICE gathering state
#### 4.4.1.5 Set the session description
#### 4.4.1.6 Set the configuration

### 4.4.2 Interface Definition
### 4.4.3 Legacy Interface Extensions
#### 4.4.3.1
### 4.4.4 Garbage collection

1. 
2. 
3. configuration.certificates がセットされていたら証明書の処理
4. configuration.bundlePolicy が接続のポリシーと違っていたらエラー
5. configuration.rtcpMuxPolicy が接続のポリシーと違っていたらエラー
6. configuration.iceCandidatePoolSize










##
##

* [Chrome M75から chrome://webrtc-internals が新しくなります](https://qiita.com/yusuke84/items/428affe75affa16f104d)
* [webrtc-dump-importer](https://github.com/fippo/webrtc-dump-importer/)

## 

#### なにを、なぜ、どのように
#### シグナリング

* [SDP for WebRTC](https://www.slideshare.net/iwashi86/webrtc-for-sdp)
* [WebRTC samples Munge SDP](https://www.slideshare.net/iwashi86/webrtc-for-sdp)

#### 接続
#### セキュリティ対策
#### リアルタイムネットワーキング
#### メディアコミュニケーション
#### データコミュニケーション
#### 応用WebRTC
#### デバッグ
#### 歴史
#### FAQ
