# 카카오TV 플랫폼 채팅 봇

### 프로젝트 소개

이 프로젝트는 카카오 TV라는 라이브 스트리밍 플랫폼에서 작동할 수 있는 전용 채팅 벗입니다.

카카오 TV에서는 다른 플랫폼과는 다르게 API를 제공하지 않기 때문에 WebSocket에 접근하고 플랫폼 내부에 사용되는 REST API를 사용하기 위해 Docker Selenium Standalone 과 Fiddler가 사용되었습니다.

이 채팅 봇은 현재 스트리밍 상태를 확인해 스트리밍이 시작될 경우 단계가 시작되고 스트리밍이 종료될 시 해당 봇은 기능을 멈추게 작동됩니다.

카카오 TV라는 플랫폼은 API를 제공하고 있지는 않지만 라이브 스트리밍을 시청하기 위한 전용 소프트웨어와 웹에서 시청할 수 있는 사이트를 제공하고 있습니다.

저는 여기서 Websocket에 접근하는 방법과 작동 방법을 찾아 채팅방에 접속했습니다.

채팅방에 접속하기 위해서는 유저의 아이디 번호와 현재 진행 중인 채팅방의 번호가 필요합니다.

그다음으로 채팅 봇이 채팅을 보낼 수 있는 REST API에 세션이 필요해 Selenium을 통한 해당 라이브 스트리밍에 접속 후 로그인 되어있는 채팅 봇 아이디의 세션 값을 가져와 봇의 기능을 할 수 있게 했습니다.

이 프로젝트를 진행하면서 이 플랫폼의 채팅의 작동 방식을 배울 수 있어서 좋았습니다.

읽을 수 있는 기능만 WebSocket을 사용하고 보내거나 명령어를 처리할 때에는 REST API를 사용해 처리하는 방식이라 나중에 한번 사용해 보고 싶습니다.