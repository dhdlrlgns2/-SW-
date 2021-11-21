# -SW-
getopt()

int getopt(int argc, char * const argv[], const char *optstring);
이 함수의 파라미터는 간단한다.

argc, argv : main() 함수가 받은 파라미터를 그대로 전달한다.
optstring : 파싱해야 할 파라미터를 쓴다. 옵션이 별도의 파라미터를 받는 경우 콜론을 함께 쓴다.
예를 들어 -h, -v, -f filename을 받는 세 가지 옵션이 있다고 하면 옵션스트링은 "hvf:"가 된다. 각각의 옵션을 파싱해내기 위해서는 getopt()함수가 0을 리턴할 때까지 계속해서 반복하면 된다.

getopts()

getopts opsting varname

쉘 에서 명령을 실행할 때 옵션을 사용하는데요. 스크립트 파일이나 함수를 실행할 때도 동일하게 옵션을 사용할 수 있습니다. 사용된 옵션은 다른 인수들과 마찬가지로 $1, $2, ... positional parameters 형태로 전달되므로 스크립트 내에서 직접 옵션을 해석해서 사용해야 됩니다. 이때 옵션 해석 작업을 쉽게 도와주는 명령이 getopts 입니다.

옵션에는 short 옵션과 long 옵션이 있는데 getopts 명령은 short 옵션을 처리합니다.

표준입력으로 값을 받아 awk 스크립트를 통해 원하는 표준출력을 내보낼 수 있다. awk는 1977년에 AT&T 연구소의 Alfred V. Aho, Peter J. Weinverger, Brian W. Kernighan 세 사람이 만들었다. awk라는 이름도 세 사람 이름의 앞 글자이다. 이후 1986년 Paul Rubin과 Jay Fenlason이 GNU 버전의 awk를 만들어서 리눅스에서 사용했다.
[네이버 지식백과] awk (유닉스 리눅스 명령어 사전, 2010. 11. 30., 우종경, 박종오)
