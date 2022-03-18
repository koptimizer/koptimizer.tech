<p align = 'center'>
   <img src="https://github.com/koptimizer/koptimizer.tech/blob/main/assets/img/icons/github_fill.svg" width="500" height="500"><br>
   <b> https://koptimizer.tech </b>
</p>
</br>

# Koptimizer.tech
- 본 repo는 [Adam Blog 2.0](http://jekyllthemes.org/themes/adam-blog-2/)을 하드포크하였으며, [MIT License](https://ko.wikipedia.org/wiki/MIT_%ED%97%88%EA%B0%80%EC%84%9C)를 갖습니다.
- koptimizer로 게시된 모든 글의 저작권은 저에게 있습니다.
</br>

### 블로그 관리 핵심파일
- ```_config.yml```을 통해서 홈페이지 title과 description, 메인 화면 텍스트를 변경할 수 있습니다.
- ```_includes/*.html``` 및 ```_layouts/default.html```  파일을 통해서 홈페이지 내부의 모든 내용을 변경할 수 있습니다.
- ```assets/css/main.css```를 통해서 요소들의 속성을 수정하고 정의해줄 수 있습니다.
- 모든 이미지는 ```assets/img/...```에 저장해서 사용해주세요.

### 온라인에서 작업하는 방법
- Github을 이용해서 해당 파일을 직접 수정하면 자동으로 commit 되어서 바로 적용됩니다.
- 실제 웹으로 적용되기까지 1~30분 가량의 시간이 걸리나 수정이 간편해서 간소한 수정에 용이합니다.

### 로컬PC에서 작업하는 방법
- 만약 첫 작업인 경우:
   - [해당 링크](https://rubyinstaller.org/downloads/)에서 Ruby+DevKit 2.x.x 버젼을 다운받습니다.
   - ruby를 설치하고, ruby prompt를 켭니다.
   - ```gem install jekyll bundler```을 실행하여 jekyll과 필요한 gem 파일을 설치합니다.
- ```$ git clone``` 혹은 ```$ git pull```을 통해 해당 레포지토리를 로컬 pc의 적절한 디렉토리로 끌어옵니다.
- Ruby prompt를 켜고 로컬 레포지토리로 이동한 후, ```jekyll serve```를 입력합니다.
- serve를 실행하면 localhost:4000에서 자신이 작업하는 홈페이지의 모습을 바로 확인할 수 있습니다.
- 모든 작업이 완료되었다면 ```commit -> push (-> pull reqeust)```을 해서 원격 레포지토리에 업로드하시면 됩니다.
- 실제 웹으로 적용되기 까지 1~30분 가량의 시간이 소요됩니다.
