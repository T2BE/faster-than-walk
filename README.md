<meta name='keywords' content='walk, python, faster, speed, benchmark, rapido, velocidad, optimizacion, cython, pypy, cpython, docker, json, ndjson, rapido, veloz, performance, critical, compiled, module, modulo, loc, minimalismo, minimalism, simple, small, tiny, argentina, spanish, compare, mejora'>

# Faster-than-Walk

[![screenshot](https://source.unsplash.com/eH_ftJYhaTY/800x402)](https://youtu.be/QiKwnlyhKrk?t=5)

| Library                       | Speed    |
|-------------------------------|----------|
| os.walk (std lib)             | `225.89` |
| Faster_than_csv               | `75.0`   |

<details>

- Benchmarks run on Docker from Dockerfile on this repo.
- Speed is IRL time to complete 10000 full recursive directory walks to `/usr/share/`.
- Stats as of year 2019.

</details>


# Use

```python
import faster_than_walk as ftw
print(ftw.walks("sample.csv"))  # See Docs for more info.
```

- `faster_than_walk.walks(folderpath: str, extensions: list, followlinks=false, yieldfiles=true, debugs=false)` Recursive directory walk from path to list of strings.
- `faster_than_walk.walks_glob(globpattern: str)` Recursive directory walk from standard POSIX like Glob Pattern string to list of strings.
- `faster_than_walk.walks_simple(folderpath: str)` Recursive directory walk from path to list of strings.


# Docker

- Make a quick test drive on Docker!.

```bash
$ ./build-docker.sh
$ ./run-docker.sh
$ ./run-benchmark.sh  # Inside Docker.
```


# Platforms

- ✅ Linux
- ✅ Windows
- ✅ Mac
- ✅ Android
- ✅ Raspberry Pi
- ✅ BSD


# FAQ

- Whats the idea, inspiration, reason, etc ?.

[Feel free to Fork, Clone, Download, Improve, Reimplement, Play with this Open Source. Make it 10 times faster, 10 times smaller.](http://tonsky.me/blog/disenchantment)

- This requires Cython ?.

No.

- This runs on PyPy ?.

No.

- This runs on Python2 ?.

I dunno. (Not supported)

- How can I Install it ?.

`pip install faster_than_walk`

- How can be faster than `os.walk` ?.

I dunno.
