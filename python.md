# Python Style Guide for AISlab

## Prerequisite
* All scripts follow [PEP8](https://www.python.org/dev/peps/pep-0008/)

## Requirement
* cookiecutter
* aislab-co/python 

## Common

## Versioning

## Indentation

함수 선언이 79자가 넘어간다면 한 줄에 하나의 인자씩 적어주고 마지막 인자 뒤 트레일링 콤마를 붙이고 Parentheses를 다음 줄에서 닫아줍니다.

auto formatter중 하나인 black의 기본 동작이기도 합니다.

```python
def func(
    if_some_variables: Optional[List[str]],
    over_the_80_width: Optional[int],
    separate_lines: bool = True,
) -> int:
    return 42

def foo(short: int) -> None:
    pass
```

## Trailing comma

## Quotes

## Assert

## Line length

## Line break

## Lint

- [pylint](https://www.pylint.org/): eslint처럼 작성된 파이썬 코드에 잘못된 부분은 없는지, 더 개선할 부분은 없는지 자동으로 검사해주는 린트 도구입니다. [`.pylintrc`](https://github.com/Rainist/python/blob/master/%7B%7Bcookiecutter.project_slug%7D%7D/.pylintrc) 파일을 통해 세부적인 옵션을 조정할 수 있습니다.
- [isort](https://github.com/timothycrosley/isort): import order를 자동으로 정렬해주는 도구입니다. [`.editorconfig`](https://github.com/Rainist/python/blob/master/%7B%7Bcookiecutter.project_slug%7D%7D/.editorconfig) 혹은 `.isort.cfg`로 세부적인 옵션을 조정할 수 있습니다.
- [black](https://github.com/ambv/black): auto formatter 중 하나입니다. [medium 아티클](https://medium.com/3yourmind/auto-formatters-for-python-8925065f9505)에서 볼 수 있듯 다른 포매터도 있지만 black을 제안하는 이유는 따로 설정해줘야 할 부분이 적으며 위에서 주장한 스타일에 가장 근접하게 동작하는 도구이기 때문입니다. 다만 포매터는 기호가 있을 수 있는 부분이며 없어도 충분히 AISlab의 스타일에 맞는 코드를 작성할 수 있기에 이는 개인에 판단에 따라 사용합니다.


