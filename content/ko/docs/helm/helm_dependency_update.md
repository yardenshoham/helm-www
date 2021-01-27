---
title: "Helm Dependency Update"
---

## helm dependency update

Chart.yaml 의 내용에 따라 charts/ 업데이트

### 개요


Chart.yaml 을 미러링하도록 온-디스크 종속성을 업데이트한다.

이 명령은 'Chart.yaml' 에 표현된 필수 차트가 'charts/' 에
있고 허용 가능한 버전인지를 확인한다. 종속성을 충족하는 최신 차트를
풀다운(pull down)하고 이전 종속성을 정리한다.

업데이트가 성공하면 종속성을 정확한 버전으로 다시
빌드하는데 사용할 수 있는 잠금파일이 생성된다.

종속성은 'Chart.yaml' 에 표시할 필요가 없다. 따라서 업데이트 명령은
차트가 (a)Chart.yaml 파일에 있지만, (b)잘못된 버전이 아니면
차트를 제거하지 않는다.


```
helm dependency update CHART [flags]
```

### 옵션

```
  -h, --help             helm dependency update 명령어에 대한 도움말
      --keyring string   공개키를 포함하는 키링 (기본값 "~/.gnupg/pubring.gpg")
      --skip-refresh     로컬 저장소 캐시를 새로 고치지 않음
      --verify           서명과 비교하여 패키지를 확인
```

### 부모 명령어에서 상속된 옵션들

```
      --debug                       장황한(verbose) 출력 활성화
      --kube-apiserver string       쿠버네티스 API 서버의 주소 및 포트
      --kube-as-group stringArray   작업에 관해 제시할 그룹. 플래그를 여러 번 사용하여 여러 그룹 지정 가능
      --kube-as-user string         작업에 관해 제시할 사용자명
      --kube-context string         사용할 kubeconfig 컨텍스트 이름
      --kube-token string           인증에 사용될 베어러(bearer) 토큰
      --kubeconfig string           kubeconfig 파일 경로
  -n, --namespace string            이 요청에 대한 네임스페이스 스코프
      --registry-config string      레지스트리 구성 파일에 대한 경로 (기본값 "~/.config/helm/registry.json")
      --repository-cache string     캐시된 저장소 색인이 포함된 파일의 경로 (기본값 "~/.cache/helm/repository")
      --repository-config string    저장소 이름 및 URL 을 포함하는 파일 경로 (기본값 "~/.config/helm/repositories.yaml")
```

### 함께 보기

* [helm dependency](helm_dependency.md)	 - 차트의 종속성을 관리

###### Auto generated by spf13/cobra on 29-Oct-2020