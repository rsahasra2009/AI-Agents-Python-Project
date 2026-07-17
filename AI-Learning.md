# AI + Python Learning Roadmap (1000 Labs)

> A hands-on journey from Python basics to AI expert. Each point = a concept + a 2-line lab setup.
> Prereqs you already have: basic Azure, basic Microsoft Foundry understanding.
>
> **How to use:** Do them in order. Check the box when the lab runs. Commit each lab to Git.
> **Global setup (do once):**
> ```bash
> # Install Python 3.12+, create a workspace venv, activate it
> python -m venv .venv && .\.venv\Scripts\activate    # Windows PowerShell
> pip install --upgrade pip ipykernel jupyter
> ```

---

## Phase 1 — Python Fundamentals (1–100)

1. **Install Python & verify** — Understand the interpreter and PATH. Lab: install Python 3.12, run `python --version` and `py -0p` to list installed versions.
2. **The REPL** — Interactive shell for quick experiments. Lab: open `python`, type `2+2`, `print("hi")`, then `exit()`.
3. **Running a script** — Difference between REPL and `.py` files. Lab: create `hello.py` with `print("Hello AI")`, run `python hello.py`.
4. **Comments & docstrings** — Documenting code with `#` and `"""..."""`. Lab: add a top-of-file docstring and inline comments to `hello.py`.
5. **Variables & assignment** — Names bound to objects, dynamic typing. Lab: assign `name`, `age`, `pi` and print them with an f-string.
6. **Numeric types** — `int`, `float`, `complex` and precision. Lab: compute `7/2`, `7//2`, `7%2`, `2**10` and print results.
7. **Strings basics** — Immutable text sequences. Lab: create a string, index, slice `s[0]`, `s[-1]`, `s[1:4]`.
8. **String methods** — `upper`, `lower`, `strip`, `replace`, `split`. Lab: clean `"  Hello, AI  "` into `"hello ai"`.
9. **f-strings & formatting** — Embed expressions in text. Lab: format a float to 2 decimals with `f"{pi:.2f}"`.
10. **Booleans & truthiness** — `True`/`False` and falsy values. Lab: test `bool("")`, `bool(0)`, `bool([1])` in the REPL.
11. **Comparison operators** — `==`, `!=`, `<`, `>=`, chaining. Lab: evaluate `1 < 2 < 3` and `3 == 3.0`.
12. **Logical operators** — `and`, `or`, `not`, short-circuiting. Lab: print results of `True and False`, `not None`.
13. **Conditionals** — `if`/`elif`/`else` branching. Lab: write a grade classifier for a score 0–100.
14. **The `input()` function** — Reading user input as strings. Lab: ask for a name and age, print a greeting.
15. **Type casting** — `int()`, `float()`, `str()`, `bool()`. Lab: convert `input()` age to `int` and add 1.
16. **Lists** — Ordered, mutable sequences. Lab: build a list of 5 numbers, append, insert, and pop one.
17. **List indexing & slicing** — Access ranges and steps. Lab: reverse a list with `nums[::-1]`.
18. **List methods** — `sort`, `reverse`, `count`, `index`, `extend`. Lab: sort a list of names alphabetically.
19. **Tuples** — Immutable ordered sequences. Lab: create a coordinate `(x, y)` and unpack it into two variables.
20. **Sets** — Unordered unique collections. Lab: find unique words in a sentence using `set()`.
21. **Set operations** — union, intersection, difference. Lab: compute common elements of two sets with `&`.
22. **Dictionaries** — Key–value mappings. Lab: build a `{name: score}` dict and look up one score.
23. **Dict methods** — `keys`, `values`, `items`, `get`. Lab: iterate a dict printing `"key -> value"`.
24. **Nested data structures** — Lists of dicts, dicts of lists. Lab: model 3 students each with name and grades list.
25. **`for` loops** — Iterating over sequences. Lab: sum a list of numbers with a loop.
26. **`range()`** — Generating numeric sequences. Lab: print even numbers 0–20 using `range(0,21,2)`.
27. **`while` loops** — Condition-based iteration. Lab: build a countdown from 10 to 1.
28. **`break` & `continue`** — Loop control flow. Lab: print numbers 1–20 but skip multiples of 3.
29. **`enumerate()`** — Index + value in loops. Lab: print a numbered list of items.
30. **`zip()`** — Iterate multiple sequences together. Lab: pair names with scores and print each.
31. **List comprehensions** — Concise list building. Lab: create squares of 1–10 in one line.
32. **Conditional comprehensions** — Filtering in comprehensions. Lab: extract even numbers from a list.
33. **Dict/set comprehensions** — Build dicts/sets concisely. Lab: map words to their lengths.
34. **Functions** — Reusable named blocks with `def`. Lab: write `add(a, b)` returning the sum.
35. **Parameters & arguments** — Positional vs keyword. Lab: call a function using keyword arguments.
36. **Default arguments** — Optional parameters. Lab: write `greet(name, msg="Hi")`.
37. **`*args` & `**kwargs`** — Variable arguments. Lab: write `total(*nums)` summing any count.
38. **Return values** — Single and multiple returns. Lab: return `(min, max)` of a list.
39. **Scope (LEGB)** — Local, enclosing, global, built-in. Lab: demonstrate a global vs local variable shadow.
40. **Lambda functions** — Anonymous inline functions. Lab: sort tuples by second element with `key=lambda x: x[1]`.
41. **`map`, `filter`, `reduce`** — Functional tools. Lab: double a list with `map`, filter evens with `filter`.
42. **Recursion** — Functions calling themselves. Lab: compute factorial recursively.
43. **Error types** — `ValueError`, `TypeError`, `KeyError`. Lab: trigger each error intentionally and read the traceback.
44. **`try`/`except`** — Handling exceptions. Lab: safely convert user input to int with a fallback.
45. **`else`/`finally`** — Full exception structure. Lab: add cleanup logic in `finally`.
46. **Raising exceptions** — `raise` custom errors. Lab: validate age and `raise ValueError` if negative.
47. **Custom exceptions** — Subclassing `Exception`. Lab: define `class InvalidScore(Exception)` and raise it.
48. **Reading files** — `open()` and context managers. Lab: read a `.txt` file with `with open(...)`.
49. **Writing files** — Write and append modes. Lab: write 5 lines to `output.txt`.
50. **File paths with `pathlib`** — Cross-platform paths. Lab: list all `.py` files with `Path('.').glob('*.py')`.
51. **CSV reading** — Structured text via `csv` module. Lab: read a CSV and print each row.
52. **JSON handling** — `json.load`/`dumps`. Lab: serialize a dict to a `.json` file and read it back.
53. **Modules** — Importing standard library. Lab: use `math.sqrt` and `random.randint`.
54. **Creating modules** — Split code into files. Lab: make `utils.py` with a function and import it.
55. **Packages** — Folders with `__init__.py`. Lab: create a package `mylib/` with two modules.
56. **`__name__ == "__main__"`** — Script vs import guard. Lab: add the guard to run test code only when executed.
57. **`datetime` module** — Dates and times. Lab: print today's date and add 7 days.
58. **`random` module** — Pseudo-randomness. Lab: simulate 10 dice rolls.
59. **`os` module** — Interacting with the OS. Lab: list files in a directory with `os.listdir`.
60. **`sys` module** — Interpreter interaction. Lab: read command-line args with `sys.argv`.
61. **Virtual environments** — Isolated dependencies. Lab: create and activate a `.venv`, install `requests`.
62. **`pip` basics** — Installing packages. Lab: `pip install rich` and pretty-print a table.
63. **`requirements.txt`** — Pinning dependencies. Lab: run `pip freeze > requirements.txt`.
64. **String formatting deep-dive** — Alignment, padding, signs. Lab: right-align numbers in a column.
65. **Ternary expressions** — Inline conditionals. Lab: assign `"even" if n%2==0 else "odd"`.
66. **Unpacking** — Star unpacking in assignments. Lab: `a, *rest = [1,2,3,4]` and print `rest`.
67. **`enumerate` with start** — Custom starting index. Lab: number a list starting at 1.
68. **Mutable vs immutable** — Object mutation semantics. Lab: show list aliasing vs tuple immutability.
69. **Identity vs equality** — `is` vs `==`. Lab: compare small ints and separate lists with both.
70. **Shallow vs deep copy** — `copy` module. Lab: copy a nested list and mutate the original.
71. **`collections.Counter`** — Counting elements. Lab: count word frequency in a paragraph.
72. **`collections.defaultdict`** — Auto-initializing dicts. Lab: group words by first letter.
73. **`collections.namedtuple`** — Lightweight records. Lab: define a `Point` namedtuple.
74. **`collections.deque`** — Fast queue/stack. Lab: implement a sliding window of last 3 values.
75. **`itertools` basics** — `count`, `cycle`, `chain`. Lab: chain two lists into one iterator.
76. **`itertools` combinatorics** — `permutations`, `combinations`. Lab: list all 2-item combos of `[A,B,C]`.
77. **Generators** — Lazy iteration with `yield`. Lab: write a generator for the first N Fibonacci numbers.
78. **Generator expressions** — Lazy comprehensions. Lab: sum squares with `sum(x*x for x in range(1000))`.
79. **Iterators & `__iter__`** — Iteration protocol. Lab: build a custom range-like iterator class.
80. **Decorators basics** — Wrapping functions. Lab: write a `@timer` decorator that prints run time.
81. **Decorators with args** — Parameterized decorators. Lab: write `@repeat(3)` that runs a function 3 times.
82. **`functools.wraps`** — Preserving metadata. Lab: fix a decorator to keep the wrapped function's name.
83. **`functools.lru_cache`** — Memoization. Lab: speed up recursive Fibonacci with `@lru_cache`.
84. **Context managers** — `with` protocol. Lab: write a class with `__enter__`/`__exit__`.
85. **`contextlib.contextmanager`** — Generator-based context. Lab: build a timing context manager.
86. **Type hints** — Annotating types. Lab: annotate `def add(a: int, b: int) -> int`.
87. **`typing` module** — `List`, `Dict`, `Optional`. Lab: type-hint a function returning `Optional[str]`.
88. **`mypy` static checking** — Catch type errors. Lab: run `mypy script.py` on annotated code.
89. **Dataclasses** — Boilerplate-free classes. Lab: define `@dataclass class Student`.
90. **Enums** — Named constants. Lab: create `class Color(Enum)` with 3 members.
91. **Classes & objects** — OOP basics with `class`. Lab: define `Dog` with `__init__` and a `bark` method.
92. **Instance vs class attributes** — Shared vs per-object. Lab: add a class-level counter of instances.
93. **`__str__` & `__repr__`** — Object representations. Lab: give `Dog` a readable `__str__`.
94. **Inheritance** — Subclassing and `super()`. Lab: make `Puppy(Dog)` overriding `bark`.
95. **Polymorphism** — Same interface, different behavior. Lab: loop over animals calling `.speak()`.
96. **Encapsulation** — Private attributes with `_`/`__`. Lab: add a private balance to a `BankAccount`.
97. **Properties** — Managed attributes with `@property`. Lab: add a computed `area` property to `Circle`.
98. **Class & static methods** — `@classmethod`, `@staticmethod`. Lab: add a `from_string` classmethod factory.
99. **Abstract base classes** — `abc` module. Lab: define an abstract `Shape` with abstract `area()`.
100. **Mini project: CLI todo app** — Combine all fundamentals. Lab: build a `todo.py` that adds/lists/removes tasks stored in JSON.

## Phase 2 — Intermediate & Advanced Python (101–180)

101. **Multiple inheritance & MRO** — Method resolution order. Lab: build a diamond hierarchy and print `Cls.__mro__`.
102. **Mixins** — Reusable behavior classes. Lab: create a `JsonMixin` adding `.to_json()`.
103. **Operator overloading** — `__add__`, `__eq__`, `__lt__`. Lab: make a `Vector` class support `+`.
104. **`__getitem__`/`__len__`** — Container protocol. Lab: build an indexable `Playlist` class.
105. **`__call__`** — Callable objects. Lab: make a `Multiplier(3)` instance callable like a function.
106. **Slots** — Memory optimization with `__slots__`. Lab: compare memory of a class with and without slots.
107. **Descriptors** — Managed attribute protocol. Lab: write a `Positive` descriptor validating values.
108. **Metaclasses** — Classes that build classes. Lab: create a metaclass that registers subclasses.
109. **Closures** — Functions capturing state. Lab: build a `make_counter()` closure.
110. **`nonlocal` keyword** — Modify enclosing scope. Lab: increment a counter inside a nested function.
111. **Partial functions** — `functools.partial`. Lab: create a `cube = partial(pow, exp=3)` style helper.
112. **`functools.reduce`** — Fold operations. Lab: compute product of a list with `reduce`.
113. **`functools.singledispatch`** — Type-based dispatch. Lab: overload a `describe` function by type.
114. **Regular expressions** — `re` pattern matching. Lab: extract all emails from text with `re.findall`.
115. **Regex groups** — Capturing subpatterns. Lab: parse a date `YYYY-MM-DD` into groups.
116. **Regex substitution** — `re.sub`. Lab: mask phone numbers in a string.
117. **String encoding** — `encode`/`decode`, UTF-8. Lab: encode a string to bytes and back.
118. **Bytes & bytearray** — Binary data types. Lab: read the first 16 bytes of a file.
119. **`struct` module** — Binary packing. Lab: pack two ints into bytes and unpack them.
120. **`enum` advanced** — `auto()`, `IntEnum`, flags. Lab: build a `Permission` IntFlag with bitwise combos.
121. **`argparse`** — CLI argument parsing. Lab: build a script accepting `--name` and `--count`.
122. **`logging` module** — Structured logs. Lab: configure logging to file with levels.
123. **Logging handlers** — Console + file handlers. Lab: log INFO to console, ERROR to file.
124. **Exceptions chaining** — `raise ... from`. Lab: wrap a low-level error in a domain error.
125. **`with` for multiple resources** — Nested context managers. Lab: open two files in one `with` statement.
126. **Assertions** — `assert` for invariants. Lab: assert a function's precondition and trigger it.
127. **Unpacking in function calls** — `*args`/`**kwargs` at call site. Lab: spread a dict into keyword arguments.
128. **Keyword-only arguments** — `*` in signatures. Lab: force `verbose` to be keyword-only.
129. **Positional-only arguments** — `/` in signatures. Lab: define `def f(a, /, b)`.
130. **Walrus operator** — Assignment expressions `:=`. Lab: read lines until empty using `while (line := input())`.
131. **Match statement** — Structural pattern matching. Lab: classify shapes by matching dict patterns.
132. **`Enum` in match** — Pattern matching enums. Lab: dispatch on a `Color` enum with `match`.
133. **`__init_subclass__`** — Customize subclass creation. Lab: auto-validate that subclasses define a field.
134. **`__post_init__`** — Dataclass post-processing. Lab: compute a derived field after init.
135. **Frozen dataclasses** — Immutable records. Lab: create `@dataclass(frozen=True)` and test mutation error.
136. **`field()` defaults** — Mutable defaults safely. Lab: use `field(default_factory=list)`.
137. **`__slots__` in dataclasses** — Slotted dataclasses. Lab: add `slots=True` and confirm no `__dict__`.
138. **Iterators vs iterables** — `iter()`/`next()`. Lab: manually iterate a list with `next()`.
139. **Generator `send`/`throw`** — Coroutine-style generators. Lab: build a running-average generator with `send`.
140. **`yield from`** — Delegating generators. Lab: flatten nested lists with `yield from`.
141. **Concurrency vs parallelism** — Conceptual difference. Lab: write notes comparing threads vs processes.
142. **`threading` basics** — OS threads. Lab: run two threads printing numbers concurrently.
143. **Thread locks** — Avoiding race conditions. Lab: protect a shared counter with a `Lock`.
144. **`concurrent.futures`** — Thread/process pools. Lab: parallelize URL fetches with `ThreadPoolExecutor`.
145. **The GIL** — Global Interpreter Lock impact. Lab: benchmark CPU-bound work in threads vs processes.
146. **`multiprocessing`** — True parallelism. Lab: compute squares across processes with a `Pool`.
147. **`asyncio` basics** — Event loop & coroutines. Lab: write an `async def main()` awaiting `asyncio.sleep`.
148. **`async`/`await`** — Awaitable coroutines. Lab: run three async tasks concurrently with `gather`.
149. **Async HTTP** — `aiohttp` requests. Lab: fetch 5 URLs concurrently and time it.
150. **Queues** — `queue.Queue` producer/consumer. Lab: build a producer/consumer with a shared queue.
151. **`subprocess`** — Running external commands. Lab: capture output of `git --version`.
152. **Environment variables** — `os.environ`, `dotenv`. Lab: load an API key from a `.env` file.
153. **`configparser`** — INI config files. Lab: read settings from `config.ini`.
154. **`pickle`** — Object serialization. Lab: pickle a dict to disk and reload it.
155. **`shelve`** — Persistent dict storage. Lab: store key-value data across runs.
156. **`sqlite3`** — Embedded SQL database. Lab: create a table, insert rows, and query them.
157. **SQL basics via Python** — CRUD operations. Lab: build a small contacts DB with insert/select/update/delete.
158. **`unittest`** — Built-in testing. Lab: write test cases for your `add` function.
159. **`pytest` basics** — Simpler testing. Lab: write `test_math.py` with assert-based tests.
160. **Pytest fixtures** — Reusable test setup. Lab: create a fixture providing sample data.
161. **Parametrized tests** — Multiple inputs. Lab: `@pytest.mark.parametrize` over several cases.
162. **Mocking** — `unittest.mock`. Lab: mock an API call in a test.
163. **Test coverage** — `pytest-cov`. Lab: measure coverage and reach 90%+.
164. **Code formatting** — `black`, `ruff format`. Lab: auto-format your project.
165. **Linting** — `ruff`/`flake8`. Lab: lint your project and fix warnings.
166. **Import sorting** — `isort`. Lab: sort imports across your package.
167. **Pre-commit hooks** — Automated checks. Lab: set up `.pre-commit-config.yaml` with black+ruff.
168. **Packaging** — `pyproject.toml`. Lab: create a minimal installable package.
169. **Building wheels** — `python -m build`. Lab: build a wheel of your package.
170. **Publishing (TestPyPI)** — Distribution. Lab: upload your package to TestPyPI with `twine`.
171. **Profiling** — `cProfile`. Lab: profile a slow function and read hotspots.
172. **Timing code** — `timeit`. Lab: compare list comp vs loop speed.
173. **Memory profiling** — `tracemalloc`. Lab: measure memory of building a big list.
174. **Debugging with `pdb`** — Breakpoints. Lab: set `breakpoint()` and step through code.
175. **VS Code debugger** — Launch configs. Lab: configure and hit a breakpoint in VS Code.
176. **Type-safe configs** — `pydantic` models. Lab: validate a settings dict with a Pydantic model.
177. **HTTP requests** — `requests` library. Lab: GET a public API and parse JSON.
178. **REST API consumption** — Query params, headers. Lab: call a weather API with an API key.
179. **Rate limiting & retries** — `tenacity`. Lab: add exponential-backoff retries to a request.
180. **Mini project: web scraper** — Combine requests + parsing. Lab: scrape a page with `BeautifulSoup` and save to CSV.

## Phase 3 — Dev Environment, Tooling & Git (181–220)

181. **VS Code setup** — Editor for Python/AI. Lab: install the Python + Jupyter extensions.
182. **Python interpreter selection** — Choosing a venv. Lab: select your `.venv` in VS Code's interpreter picker.
183. **Jupyter notebooks** — Interactive computing. Lab: create `intro.ipynb` and run a cell.
184. **Notebook kernels** — Connecting venvs. Lab: register your venv as a Jupyter kernel with `ipykernel`.
185. **Markdown in notebooks** — Documenting analysis. Lab: add a title and notes cell above code.
186. **Magic commands** — `%timeit`, `%matplotlib`. Lab: time a cell with `%%timeit`.
187. **JupyterLab** — Full IDE experience. Lab: launch `jupyter lab` and open a notebook.
188. **Git basics** — Version control fundamentals. Lab: `git init`, stage, and commit your project.
189. **Git branches** — Parallel development. Lab: create a `feature` branch and merge it.
190. **`.gitignore`** — Excluding files. Lab: ignore `.venv/`, `__pycache__/`, and `.env`.
191. **GitHub** — Remote repositories. Lab: push your repo to GitHub.
192. **Pull requests** — Code review flow. Lab: open a PR from a branch and merge it.
193. **Git rebase vs merge** — History strategies. Lab: rebase a feature branch onto main.
194. **Resolving conflicts** — Merge conflict handling. Lab: create and resolve a conflict on purpose.
195. **Conda vs venv** — Environment managers. Lab: create a conda env and list packages.
196. **`uv` package manager** — Fast dependency tooling. Lab: `uv venv` and `uv pip install numpy`.
197. **Dependency locking** — Reproducible builds. Lab: generate a lockfile with `pip-tools` or `uv`.
198. **Docker basics** — Containerization. Lab: write a `Dockerfile` for a Python script and build it.
199. **Running containers** — `docker run`. Lab: run your image and see the script output.
200. **Docker Compose** — Multi-service apps. Lab: define a `docker-compose.yml` with app + database.
201. **Makefiles / task runners** — Automation. Lab: add `make test` and `make format` targets.
202. **Environment secrets** — Managing keys safely. Lab: store secrets in `.env`, never commit them.
203. **WSL for Windows** — Linux dev on Windows. Lab: install WSL2 and run Python inside Ubuntu.
204. **Shell basics** — Navigating with the terminal. Lab: use `cd`, `ls`, `mkdir`, `mv` to organize files.
205. **PowerShell scripting** — Automation on Windows. Lab: write a `.ps1` that activates venv and runs a script.
206. **SSH keys** — Secure GitHub auth. Lab: generate an SSH key and add it to GitHub.
207. **GitHub Copilot** — AI pair programming. Lab: accept a Copilot suggestion in VS Code.
208. **Notebook version control** — `nbstripout`/`jupytext`. Lab: strip outputs before committing a notebook.
209. **Reproducible seeds** — Deterministic runs. Lab: set `random`/`numpy` seeds and confirm identical outputs.
210. **Project structure** — `src/` layout, tests, data. Lab: scaffold a clean AI project folder layout.
211. **README-driven dev** — Documenting projects. Lab: write a README with setup and usage.
212. **Semantic versioning** — Version numbering. Lab: tag your repo `v0.1.0`.
213. **CI with GitHub Actions** — Automated testing. Lab: add a workflow running `pytest` on push.
214. **Linting in CI** — Enforcing quality. Lab: add ruff+black checks to the CI workflow.
215. **Caching in CI** — Faster pipelines. Lab: cache pip dependencies in Actions.
216. **Environment reproducibility** — `requirements`/`environment.yml`. Lab: recreate your env on a clean machine.
217. **Jupyter in VS Code** — Integrated notebooks. Lab: run and debug a notebook cell in VS Code.
218. **Remote dev** — Codespaces / SSH remote. Lab: open your repo in a GitHub Codespace.
219. **GPU environment check** — CUDA availability. Lab: run `nvidia-smi` (or note CPU-only) and record specs.
220. **Mini project: reproducible template** — A ready-to-clone AI repo. Lab: build a cookiecutter-style template with venv, tests, CI, README.

## Phase 4 — Mathematics for AI (221–300)

221. **Why math for AI** — Role of linear algebra, calculus, stats. Lab: write notes mapping each field to an ML use.
222. **Scalars, vectors, matrices** — Core objects. Lab: create each with NumPy and print shapes.
223. **Vector addition** — Elementwise ops. Lab: add two vectors in NumPy and by hand.
224. **Scalar multiplication** — Scaling vectors. Lab: multiply a vector by 3 and plot before/after.
225. **Dot product** — Similarity & projection. Lab: compute `np.dot(a, b)` and interpret sign.
226. **Vector norms** — L1, L2, magnitude. Lab: compute `np.linalg.norm` for L1 and L2.
227. **Unit vectors** — Normalization. Lab: normalize a vector to length 1.
228. **Cosine similarity** — Angle between vectors. Lab: compute cosine similarity of two word-like vectors.
229. **Matrix multiplication** — Composition of transforms. Lab: multiply two matrices with `@` and verify by hand.
230. **Identity & inverse** — Neutral and reversing matrices. Lab: invert a 2×2 matrix and multiply back to identity.
231. **Transpose** — Row/column swap. Lab: transpose a matrix and confirm `(A^T)^T = A`.
232. **Determinant** — Volume scaling & invertibility. Lab: compute `np.linalg.det` for a singular vs non-singular matrix.
233. **Systems of equations** — `Ax = b`. Lab: solve a 2-variable system with `np.linalg.solve`.
234. **Linear independence** — Rank concept. Lab: compute `np.linalg.matrix_rank` of dependent rows.
235. **Eigenvalues & eigenvectors** — Invariant directions. Lab: compute eigenpairs of a 2×2 matrix.
236. **Eigen decomposition** — Diagonalization. Lab: reconstruct a matrix from its eigen decomposition.
237. **Singular Value Decomposition** — Factorization for ML. Lab: run `np.linalg.svd` on a small matrix.
238. **Matrix as transformation** — Geometric intuition. Lab: apply a rotation matrix to points and plot.
239. **Projections** — Projecting onto subspaces. Lab: project a vector onto another and plot the residual.
240. **Orthogonality** — Perpendicular vectors. Lab: verify two vectors are orthogonal via dot product = 0.
241. **Basis & span** — Coordinate systems. Lab: express a vector in a new basis.
242. **Trace** — Sum of diagonal. Lab: compute `np.trace` and relate to eigenvalue sum.
243. **Functions & graphs** — Mapping inputs to outputs. Lab: plot `y = x^2` with Matplotlib.
244. **Limits** — Approaching values. Lab: numerically approximate a limit as `x → 0`.
245. **Derivatives** — Rate of change. Lab: numerically estimate the derivative of `x^2` at `x=3`.
246. **Rules of differentiation** — Power, product, chain. Lab: differentiate `(3x^2+2)^2` by hand and verify with SymPy.
247. **Partial derivatives** — Multivariable gradients. Lab: compute ∂f/∂x and ∂f/∂y for `f=x^2+y^2` with SymPy.
248. **The gradient** — Direction of steepest ascent. Lab: compute and plot the gradient field of a surface.
249. **Chain rule for backprop** — Composed derivatives. Lab: derive the derivative of `sigmoid(wx+b)` step by step.
250. **Gradient descent** — Iterative minimization. Lab: minimize `f(x)=x^2` with a manual descent loop.
251. **Learning rate** — Step size effects. Lab: run descent with 3 learning rates and compare convergence.
252. **Local vs global minima** — Optimization pitfalls. Lab: minimize a bumpy function and observe getting stuck.
253. **Convex functions** — Well-behaved optimization. Lab: visualize a convex vs non-convex curve.
254. **Jacobian** — Matrix of partials. Lab: compute a Jacobian with SymPy for a 2→2 function.
255. **Hessian** — Second-order curvature. Lab: compute the Hessian of `x^2+y^2`.
256. **Integrals (concept)** — Area under curves. Lab: numerically integrate `x^2` from 0 to 1.
257. **SymPy basics** — Symbolic math. Lab: `sympy.diff` and `sympy.integrate` a polynomial.
258. **Probability basics** — Sample space & events. Lab: simulate coin flips and estimate P(head).
259. **Conditional probability** — P(A|B). Lab: estimate conditional probability from simulated data.
260. **Bayes' theorem** — Updating beliefs. Lab: compute a disease-test posterior probability.
261. **Independence** — Events not affecting each other. Lab: test independence of two simulated dice.
262. **Random variables** — Discrete vs continuous. Lab: sample from a discrete distribution with NumPy.
263. **Expected value** — Mean of a distribution. Lab: compute E[X] for a dice roll analytically and empirically.
264. **Variance & std dev** — Spread measures. Lab: compute variance of a sample two ways.
265. **Uniform distribution** — Equal likelihood. Lab: sample and histogram a uniform distribution.
266. **Normal distribution** — The bell curve. Lab: sample `np.random.normal` and plot a histogram.
267. **Binomial distribution** — Counts of successes. Lab: simulate 1000 sets of 10 coin flips.
268. **Poisson distribution** — Rare event counts. Lab: model arrivals per minute with Poisson.
269. **Central Limit Theorem** — Sampling distributions. Lab: average many samples and watch normality emerge.
270. **Law of large numbers** — Convergence to mean. Lab: plot running mean of dice rolls stabilizing.
271. **Sampling** — Drawing representative data. Lab: take random and stratified samples from a dataset.
272. **Descriptive statistics** — Mean, median, mode. Lab: compute all three on a dataset.
273. **Percentiles & quartiles** — Data spread. Lab: compute quartiles and IQR with NumPy.
274. **Correlation** — Linear association. Lab: compute Pearson correlation of two columns.
275. **Covariance** — Joint variability. Lab: compute a covariance matrix with NumPy.
276. **Hypothesis testing** — Null vs alternative. Lab: run a t-test with `scipy.stats.ttest_ind`.
277. **p-values** — Statistical significance. Lab: interpret a p-value from a simulated experiment.
278. **Confidence intervals** — Estimation ranges. Lab: compute a 95% CI for a sample mean.
279. **A/B testing** — Comparing variants. Lab: simulate two conversion rates and test the difference.
280. **Distributions in SciPy** — `scipy.stats`. Lab: fit a normal distribution to data.
281. **Maximum likelihood** — Parameter estimation. Lab: estimate the mean of data via MLE by hand.
282. **Log & exp functions** — Growth/decay & log-likelihood. Lab: plot `exp` and `log`, note inverse relation.
283. **Softmax math** — Turning scores into probabilities. Lab: implement softmax in NumPy and verify it sums to 1.
284. **Sigmoid & logits** — Squashing to (0,1). Lab: plot sigmoid and its derivative.
285. **Entropy** — Measuring uncertainty. Lab: compute entropy of a probability distribution.
286. **Cross-entropy** — Comparing distributions. Lab: compute cross-entropy between true and predicted labels.
287. **KL divergence** — Distribution distance. Lab: compute KL divergence between two distributions.
288. **Distance metrics** — Euclidean, Manhattan, cosine. Lab: compute all three between two points.
289. **Vectorization** — Replacing loops with array math. Lab: rewrite a Python loop sum as a NumPy operation and time both.
290. **Broadcasting math** — Shape-compatible ops. Lab: add a vector to each row of a matrix.
291. **Matrix calculus for ML** — Gradients of loss w.r.t. weights. Lab: derive the gradient of MSE for linear regression.
292. **Numerical stability** — Avoiding overflow. Lab: implement the log-sum-exp trick.
293. **Optimization landscape** — Saddle points & plateaus. Lab: visualize a saddle surface in 3D.
294. **Regularization math** — L1/L2 penalties. Lab: plot how L2 shrinks weights on a toy loss.
295. **Curve fitting** — `scipy.optimize.curve_fit`. Lab: fit an exponential curve to noisy data.
296. **Interpolation** — Estimating between points. Lab: interpolate missing values with SciPy.
297. **Fourier transform (intro)** — Frequency decomposition. Lab: run an FFT on a sine wave and plot spectrum.
298. **Linear regression from scratch (math)** — Normal equation. Lab: solve `θ = (XᵀX)⁻¹Xᵀy` in NumPy.
299. **Gradient descent from scratch** — Full training loop math. Lab: fit a line to data using manual gradient updates.
300. **Mini project: math playground** — Consolidate the math. Lab: notebook implementing gradient descent + visualizing the loss surface.

## Phase 5 — NumPy & Numerical Computing (301–360)

301. **NumPy install & import** — The array library. Lab: `pip install numpy`, import as `np`, print version.
302. **Creating arrays** — `array`, `zeros`, `ones`. Lab: build a 3×3 zeros and a 1D range array.
303. **`arange` & `linspace`** — Numeric ranges. Lab: create 50 evenly spaced points 0–1.
304. **Array attributes** — `shape`, `dtype`, `ndim`. Lab: inspect a 2D array's attributes.
305. **Reshaping** — `reshape`, `ravel`, `flatten`. Lab: reshape a 12-element array to 3×4.
306. **Indexing** — Element and row/column access. Lab: extract a specific element and a full column.
307. **Slicing** — Sub-array views. Lab: slice the top-left 2×2 of a matrix.
308. **Boolean masking** — Conditional selection. Lab: select all values > 0 from an array.
309. **Fancy indexing** — Index arrays. Lab: pick rows `[0,2,4]` from a matrix.
310. **Broadcasting** — Auto-expanding shapes. Lab: subtract a column mean from each row.
311. **Elementwise ops** — Vectorized arithmetic. Lab: compute `a*b + c` on three arrays.
312. **Aggregations** — `sum`, `mean`, `max`, `min`. Lab: compute row-wise and column-wise means.
313. **Axis argument** — Directional reductions. Lab: sum along `axis=0` vs `axis=1`.
314. **Universal functions** — `np.sqrt`, `np.exp`. Lab: apply `np.exp` to an array.
315. **Random module** — `np.random`. Lab: generate a 3×3 matrix of random numbers with a seed.
316. **Random distributions** — normal, uniform, choice. Lab: sample 1000 normal values and histogram them.
317. **Sorting** — `np.sort`, `argsort`. Lab: sort an array and get sort indices.
318. **Unique & counts** — `np.unique`. Lab: count unique labels in an array.
319. **Stacking** — `vstack`, `hstack`, `concatenate`. Lab: stack two arrays vertically and horizontally.
320. **Splitting** — `split`, `hsplit`. Lab: split an array into 3 parts.
321. **Matrix ops** — `@`, `dot`, `matmul`. Lab: multiply two matrices.
322. **Linear algebra** — `np.linalg` suite. Lab: solve a linear system and compute a determinant.
323. **Copy vs view** — Memory semantics. Lab: modify a slice and observe the original changing.
324. **`np.where`** — Vectorized conditionals. Lab: replace negatives with 0 using `np.where`.
325. **Clipping** — Bounding values. Lab: clip an array to `[0, 1]`.
326. **NaN handling** — `np.nan`, `nanmean`. Lab: compute a mean ignoring NaNs.
327. **Type casting** — `astype`. Lab: convert a float array to int.
328. **Save & load** — `np.save`/`np.load`. Lab: persist an array to `.npy` and reload it.
329. **Memory layout** — C vs Fortran order. Lab: compare `.flags` of two arrays.
330. **Performance timing** — Vectorized vs loop. Lab: benchmark a loop vs vectorized sum.
331. **Meshgrid** — Coordinate grids. Lab: build a grid and evaluate a 2D function on it.
332. **Cumulative ops** — `cumsum`, `cumprod`. Lab: compute a running total of an array.
333. **Outer product** — `np.outer`. Lab: build a multiplication table via outer product.
334. **Element counting** — `bincount`, histograms. Lab: histogram integer labels.
335. **Percentiles** — `np.percentile`. Lab: compute the 90th percentile of data.
336. **Normalization** — Min-max & z-score. Lab: normalize an array to zero mean, unit variance.
337. **Distance matrices** — Pairwise distances. Lab: compute pairwise Euclidean distances via broadcasting.
338. **Masked arrays** — `np.ma`. Lab: mask invalid entries and compute a mean.
339. **Structured arrays** — Named fields. Lab: build an array with `name` and `age` fields.
340. **Vectorizing custom funcs** — `np.vectorize`. Lab: vectorize a Python scalar function.
341. **Einstein summation** — `np.einsum`. Lab: compute a matrix product with `einsum`.
342. **Tensordot** — Higher-dim contractions. Lab: contract two 3D arrays.
343. **Random seeds & Generators** — `default_rng`. Lab: create a reproducible RNG and sample.
344. **Simulating data** — Synthetic datasets. Lab: generate a noisy linear dataset with NumPy.
345. **Monte Carlo** — Estimation by sampling. Lab: estimate π by sampling points in a square.
346. **Image as array** — Pixels as numbers. Lab: load an image into a NumPy array and print its shape.
347. **Image manipulation** — Slicing pixels. Lab: crop and flip an image via array slicing.
348. **Grayscale conversion** — Channel math. Lab: convert RGB to grayscale with a weighted sum.
349. **Convolution (manual)** — Sliding kernels. Lab: apply a blur kernel to an image manually.
350. **Signal generation** — Sine waves. Lab: generate and plot a composite sine signal.
351. **FFT with NumPy** — Frequency analysis. Lab: FFT a noisy signal and identify its frequency.
352. **Polynomials** — `np.polyfit`/`polyval`. Lab: fit a degree-2 polynomial to points.
353. **Gradient (numeric)** — `np.gradient`. Lab: compute the numeric gradient of a sampled function.
354. **Tiling & repeating** — `np.tile`, `repeat`. Lab: tile a small pattern into a larger array.
355. **Advanced reshaping** — `newaxis`, `expand_dims`. Lab: add a channel dimension to an image array.
356. **Boolean reductions** — `any`, `all`. Lab: check if any value exceeds a threshold.
357. **Argmax/argmin** — Locating extremes. Lab: find the index of the max value per row.
358. **Set operations** — `intersect1d`, `union1d`. Lab: find common elements of two arrays.
359. **Memory-efficient dtypes** — float32 vs float64. Lab: compare memory of the same array in two dtypes.
360. **Mini project: NumPy image filters** — Apply real filters. Lab: build blur, sharpen, and edge-detect kernels on an image.

## Phase 6 — Pandas & Data Wrangling (361–460)

361. **Pandas intro** — Tabular data toolkit. Lab: `pip install pandas`, import, print version.
362. **Series** — 1D labeled arrays. Lab: create a Series of scores with a custom index.
363. **DataFrames** — 2D labeled tables. Lab: build a DataFrame from a dict of lists.
364. **Reading CSV** — `read_csv`. Lab: load a CSV and call `.head()`.
365. **Reading Excel** — `read_excel`. Lab: load an `.xlsx` sheet into a DataFrame.
366. **Reading JSON** — `read_json`. Lab: load nested JSON into a DataFrame.
367. **Inspecting data** — `head`, `tail`, `info`, `describe`. Lab: profile a dataset with all four.
368. **Selecting columns** — Bracket & dot access. Lab: select two columns as a sub-DataFrame.
369. **Selecting rows** — `loc` vs `iloc`. Lab: get rows 10–20 with `iloc` and by label with `loc`.
370. **Boolean filtering** — Conditional rows. Lab: filter rows where a column > threshold.
371. **Multiple conditions** — `&`, `|`. Lab: filter with two combined conditions.
372. **`query()` method** — Readable filtering. Lab: filter rows using `df.query("age > 30")`.
373. **Adding columns** — Derived features. Lab: add a BMI column computed from weight and height.
374. **Dropping columns/rows** — `drop`. Lab: drop an unneeded column and a bad row.
375. **Renaming** — `rename`. Lab: rename columns to snake_case.
376. **Handling missing data** — `isna`, `dropna`, `fillna`. Lab: fill missing values with the column mean.
377. **Duplicates** — `duplicated`, `drop_duplicates`. Lab: remove duplicate rows.
378. **Data types** — `dtypes`, `astype`. Lab: convert a string column to datetime.
379. **String operations** — `.str` accessor. Lab: lowercase and strip a text column.
380. **Datetime handling** — `to_datetime`, `.dt`. Lab: extract year and month from a date column.
381. **Sorting** — `sort_values`, `sort_index`. Lab: sort by two columns descending.
382. **`apply()`** — Row/column functions. Lab: apply a custom function to a column.
383. **`map()` on Series** — Value mapping. Lab: map category codes to labels.
384. **`replace()`** — Value substitution. Lab: replace placeholder values with NaN.
385. **`groupby` basics** — Split-apply-combine. Lab: group by category and compute mean.
386. **Group aggregations** — `agg` with multiple funcs. Lab: get mean and count per group.
387. **`pivot_table`** — Cross-tabulated summaries. Lab: pivot sales by region and month.
388. **`crosstab`** — Frequency tables. Lab: cross-tabulate two categorical columns.
389. **Merging** — `merge` (SQL-style joins). Lab: inner-join two DataFrames on a key.
390. **Join types** — inner, left, right, outer. Lab: compare row counts across all four join types.
391. **Concatenation** — `concat`. Lab: stack two DataFrames vertically.
392. **`melt`** — Wide to long. Lab: melt a wide table into tidy long format.
393. **`pivot`** — Long to wide. Lab: pivot long data back to wide.
394. **MultiIndex** — Hierarchical indexing. Lab: create and slice a two-level index.
395. **Resetting index** — `reset_index`. Lab: flatten a grouped result back to columns.
396. **Window functions** — `rolling`, `expanding`. Lab: compute a 7-day rolling average.
397. **Shifting** — `shift`, `diff`. Lab: compute day-over-day change of a column.
398. **Categorical dtype** — Memory & speed. Lab: convert a repeated string column to category.
399. **Binning** — `cut`, `qcut`. Lab: bin ages into groups with `pd.cut`.
400. **Value counts** — Frequency of categories. Lab: get the top 5 most common values.
401. **Correlation matrix** — `df.corr()`. Lab: compute and inspect correlations.
402. **Sampling** — `sample`. Lab: draw a random 10% sample.
403. **Chaining methods** — Fluent pipelines. Lab: filter → group → aggregate in one chain.
404. **`pipe()`** — Custom pipeline steps. Lab: insert a custom cleaning function via `pipe`.
405. **Exporting data** — `to_csv`, `to_excel`, `to_parquet`. Lab: save a cleaned DataFrame to Parquet.
406. **Reading from SQL** — `read_sql`. Lab: query a SQLite DB into a DataFrame.
407. **Writing to SQL** — `to_sql`. Lab: save a DataFrame to a SQLite table.
408. **Reading from URL/API** — Remote data. Lab: load a CSV directly from a URL.
409. **Chunked reading** — Large files. Lab: read a big CSV in chunks and aggregate.
410. **Performance dtypes** — Downcasting. Lab: reduce memory with `pd.to_numeric(downcast=...)`.
411. **`eval`/`query` speed** — Fast expressions. Lab: benchmark `eval` vs standard arithmetic.
412. **Handling outliers** — IQR method. Lab: filter rows outside 1.5×IQR.
413. **Data validation** — `pandera` schemas. Lab: define and validate a DataFrame schema.
414. **Datetime indexing** — Time-series slicing. Lab: set a datetime index and slice a date range.
415. **Resampling** — `resample`. Lab: downsample hourly data to daily means.
416. **Time zones** — `tz_localize`, `tz_convert`. Lab: convert timestamps between time zones.
417. **Missing-time interpolation** — Filling gaps. Lab: interpolate a gappy time series.
418. **`explode`** — List-column expansion. Lab: explode a column of lists into rows.
419. **`get_dummies`** — One-hot encoding. Lab: one-hot encode a categorical column.
420. **`factorize`** — Label encoding. Lab: encode categories to integer codes.
421. **Styling DataFrames** — `.style`. Lab: highlight max values in a table.
422. **Memory profiling** — `memory_usage`. Lab: measure a DataFrame's memory footprint.
423. **Vectorized string parsing** — Regex extract. Lab: extract area codes from phone numbers.
424. **Conditional columns** — `np.select`. Lab: create a tier column from value ranges.
425. **Cumulative group ops** — `groupby.cumsum`. Lab: running total within each group.
426. **Rank** — `rank`. Lab: rank students within each class.
427. **`nlargest`/`nsmallest`** — Top-k rows. Lab: get the 3 highest-revenue rows per region.
428. **Cross-column apply** — Row-wise logic. Lab: compute a score from multiple columns with `apply(axis=1)`.
429. **DataFrame merging pitfalls** — Key duplication. Lab: reproduce and fix a many-to-many join blowup.
430. **Tidy data principles** — One variable per column. Lab: reshape a messy table into tidy form.
431. **Reading messy CSVs** — Bad delimiters, encodings. Lab: parse a semicolon-separated latin-1 file.
432. **Combining many files** — `glob` + concat. Lab: read all CSVs in a folder into one DataFrame.
433. **Aggregation with named outputs** — Named agg. Lab: produce clearly named summary columns.
434. **Percent change over groups** — Growth metrics. Lab: compute month-over-month growth per product.
435. **Cohort-style pivots** — Retention tables. Lab: build a simple signup-month cohort table.
436. **DataFrame equality testing** — `assert_frame_equal`. Lab: unit-test a transformation function.
437. **Handling mixed types** — Coercion issues. Lab: clean a column with mixed strings and numbers.
438. **Currency/number parsing** — Removing symbols. Lab: parse `"$1,234.50"` into a float column.
439. **Boolean to numeric** — Encoding flags. Lab: convert True/False to 1/0 for modeling.
440. **Feature-ready export** — Final clean dataset. Lab: produce a model-ready Parquet file with no NaNs.
441. **Polars intro** — Fast DataFrame alternative. Lab: read a CSV with Polars and compare speed to Pandas.
442. **Lazy evaluation** — Polars query plans. Lab: build a lazy Polars pipeline and `.collect()`.
443. **Dask intro** — Out-of-core data. Lab: load a large CSV with Dask and compute a mean.
444. **DuckDB + Pandas** — SQL on DataFrames. Lab: query a DataFrame with DuckDB SQL.
445. **Parquet & columnar formats** — Efficient storage. Lab: compare CSV vs Parquet file size and read time.
446. **Data profiling reports** — `ydata-profiling`. Lab: generate an automated EDA report.
447. **Schema inference** — Robust loading. Lab: specify dtypes explicitly on load to avoid surprises.
448. **Joining time series** — `merge_asof`. Lab: align two time series by nearest timestamp.
449. **Deduplication strategies** — Keeping latest. Lab: keep the most recent record per user.
450. **Aggregating text** — Concatenating groups. Lab: join all comments per user into one string.
451. **Pivot with multiple values** — Multi-metric pivots. Lab: pivot both count and sum together.
452. **Handling high cardinality** — Rare category grouping. Lab: bucket rare categories into "Other".
453. **Data leakage awareness** — Train/test contamination. Lab: identify a leaky feature in a sample dataset.
454. **Reproducible pipelines** — Deterministic transforms. Lab: wrap cleaning steps into a reusable function.
455. **Reading APIs into Pandas** — `json_normalize`. Lab: flatten nested API JSON into a table.
456. **Working with geospatial-ish data** — Lat/long columns. Lab: compute distances between coordinate pairs.
457. **Sampling for balance** — Under/oversampling. Lab: balance a class column by resampling.
458. **Data versioning concept** — Snapshotting datasets. Lab: save timestamped dataset versions.
459. **EDA checklist** — Systematic exploration. Lab: write and run a reusable EDA notebook template.
460. **Mini project: end-to-end cleaning** — Real messy dataset. Lab: take a raw Kaggle CSV to a clean, documented Parquet file.

## Phase 7 — Data Visualization (461–520)

461. **Matplotlib intro** — Core plotting library. Lab: plot a simple line chart of a list.
462. **Figure & axes** — Object-oriented API. Lab: create a fig/ax and plot on the axes.
463. **Line plots** — Trends over x. Lab: plot two lines with a legend.
464. **Scatter plots** — Relationships. Lab: scatter two columns colored by a third.
465. **Bar charts** — Category comparison. Lab: bar-chart counts per category.
466. **Histograms** — Distribution shape. Lab: histogram a numeric column with 30 bins.
467. **Box plots** — Spread & outliers. Lab: box-plot a metric across categories.
468. **Pie charts** — Proportions (used sparingly). Lab: pie-chart category shares.
469. **Subplots** — Multiple panels. Lab: build a 2×2 grid of related charts.
470. **Titles & labels** — Chart annotation. Lab: add title, axis labels, and legend to a plot.
471. **Colors & styles** — Visual encoding. Lab: apply a colormap and marker styles.
472. **Ticks & formatting** — Axis control. Lab: format the y-axis as percentages.
473. **Annotations** — Callouts on plots. Lab: annotate the max point with an arrow.
474. **Saving figures** — `savefig`. Lab: export a chart to PNG at 300 DPI.
475. **Styles/themes** — `plt.style`. Lab: apply the `ggplot` style.
476. **Twin axes** — Dual y-axes. Lab: plot two series with different scales.
477. **Log scales** — Wide-range data. Lab: plot data on a log-y axis.
478. **Error bars** — Uncertainty display. Lab: add error bars to a mean plot.
479. **Fill between** — Shaded regions. Lab: shade a confidence band around a line.
480. **Seaborn intro** — Statistical plotting. Lab: `pip install seaborn`, load a built-in dataset.
481. **Seaborn scatter/relplot** — Faceted relationships. Lab: relplot with hue and size mappings.
482. **Seaborn histplot/kdeplot** — Distributions. Lab: overlay a histogram with a KDE curve.
483. **Seaborn boxplot/violinplot** — Group distributions. Lab: violin-plot a metric across groups.
484. **Seaborn heatmap** — Matrix visualization. Lab: heatmap a correlation matrix.
485. **Seaborn pairplot** — Multivariate overview. Lab: pairplot a small dataset colored by class.
486. **Seaborn regplot/lmplot** — Regression lines. Lab: plot a scatter with a fitted regression line.
487. **Seaborn countplot** — Category counts. Lab: countplot a categorical column.
488. **FacetGrid** — Small multiples. Lab: facet a plot across a categorical variable.
489. **Color palettes** — Perceptual palettes. Lab: apply a colorblind-safe palette.
490. **Plotly intro** — Interactive charts. Lab: `pip install plotly`, make an interactive scatter.
491. **Plotly hover & zoom** — Interactivity. Lab: add custom hover text to points.
492. **Plotly Express** — Quick interactive plots. Lab: `px.line` a time series.
493. **Plotly 3D** — Three-dimensional plots. Lab: 3D-scatter a dataset.
494. **Plotly dashboards intro** — Layout of charts. Lab: arrange two charts in one figure.
495. **Interactive widgets** — `ipywidgets`. Lab: add a slider to control a plot parameter.
496. **Geographic maps** — `plotly`/`folium`. Lab: plot points on a world map.
497. **Choropleth maps** — Region coloring. Lab: color countries by a metric.
498. **Time-series plotting** — Date axes. Lab: plot a resampled time series with formatted dates.
499. **Distribution comparison** — Overlaid KDEs. Lab: compare two groups' distributions on one axis.
500. **Correlation heatmaps (annotated)** — Readable matrices. Lab: annotate a heatmap with values.
501. **Pairwise scatter matrix** — Feature relationships. Lab: build a scatter matrix of 4 features.
502. **Categorical plots** — Grouped bars. Lab: grouped bar chart across two categories.
503. **Stacked bar/area** — Part-to-whole over time. Lab: stacked-area chart of category shares over time.
504. **Annotated line charts** — Event markers. Lab: mark key events on a trend line.
505. **Residual plots** — Model diagnostics. Lab: plot residuals of a linear fit.
506. **Learning curve plots** — Train vs val over epochs. Lab: plot a loss curve from a dict of values.
507. **Confusion matrix plot** — Classification results. Lab: visualize a confusion matrix with a heatmap.
508. **ROC curve plot** — Classifier tradeoffs. Lab: plot an ROC curve from scores.
509. **Feature importance plot** — Model interpretation. Lab: bar-chart feature importances.
510. **Dimensionality plots** — 2D embeddings. Lab: scatter a PCA/t-SNE 2D projection colored by label.
511. **Word clouds** — Text frequency viz. Lab: generate a word cloud from a corpus.
512. **Dashboards with Streamlit** — Data apps. Lab: `pip install streamlit`, build a one-chart app.
513. **Streamlit widgets** — Interactivity. Lab: add a selectbox that filters the chart.
514. **Streamlit layout** — Columns & tabs. Lab: arrange charts in columns.
515. **Gradio for ML demos** — Quick UIs. Lab: wrap a function in a Gradio interface.
516. **Chart accessibility** — Color & labels. Lab: audit a chart for colorblind safety and add labels.
517. **Storytelling with data** — Narrative charts. Lab: build a 3-chart story answering one question.
518. **Exporting reports** — Notebook to HTML/PDF. Lab: export an analysis notebook to HTML.
519. **Publication-quality figures** — Fonts, DPI, sizing. Lab: produce a polished figure for a report.
520. **Mini project: interactive dashboard** — Combine everything. Lab: build a Streamlit dashboard exploring a real dataset.

## Phase 8 — Classical Machine Learning (521–660)

521. **What is ML** — Learning from data vs rules. Lab: write notes contrasting ML with traditional programming.
522. **Types of ML** — Supervised, unsupervised, RL. Lab: categorize 5 real problems by ML type.
523. **The ML workflow** — Data → model → evaluate → deploy. Lab: diagram the workflow for a chosen problem.
524. **scikit-learn intro** — The classical ML library. Lab: `pip install scikit-learn`, import, print version.
525. **Toy datasets** — `load_iris`, `load_digits`. Lab: load Iris and inspect features/targets.
526. **Features & labels** — X and y. Lab: split a DataFrame into `X` and `y`.
527. **Train/test split** — Held-out evaluation. Lab: `train_test_split` with an 80/20 ratio.
528. **The estimator API** — `fit`/`predict`. Lab: fit any model and predict on test data.
529. **Linear regression** — Predicting continuous values. Lab: fit `LinearRegression` on a housing-like dataset.
530. **Interpreting coefficients** — Feature effects. Lab: print and interpret regression coefficients.
531. **MSE, RMSE, MAE** — Regression metrics. Lab: compute all three on predictions.
532. **R² score** — Explained variance. Lab: compute `r2_score` for your model.
533. **Polynomial regression** — Nonlinear fits. Lab: fit degree-3 features with `PolynomialFeatures`.
534. **Overfitting & underfitting** — Bias–variance. Lab: compare train vs test error across polynomial degrees.
535. **Ridge regression** — L2 regularization. Lab: fit `Ridge` and compare to plain regression.
536. **Lasso regression** — L1 & feature selection. Lab: fit `Lasso` and see coefficients shrink to zero.
537. **ElasticNet** — Combined L1/L2. Lab: tune the L1 ratio and compare.
538. **Logistic regression** — Binary classification. Lab: classify a binary dataset with `LogisticRegression`.
539. **Decision boundary** — Visualizing classifiers. Lab: plot a 2D decision boundary.
540. **Accuracy, precision, recall** — Classification metrics. Lab: compute all three with `classification_report`.
541. **F1 score** — Balancing precision/recall. Lab: compute F1 for an imbalanced dataset.
542. **Confusion matrix** — Error breakdown. Lab: compute and plot a confusion matrix.
543. **ROC & AUC** — Threshold-independent evaluation. Lab: compute AUC and plot the ROC curve.
544. **Precision-recall curve** — Imbalanced eval. Lab: plot a PR curve for a rare-class problem.
545. **k-Nearest Neighbors** — Instance-based learning. Lab: fit `KNeighborsClassifier` and tune k.
546. **Naive Bayes** — Probabilistic classification. Lab: classify text with `MultinomialNB`.
547. **Decision trees** — Rule-based splits. Lab: fit and visualize a `DecisionTreeClassifier`.
548. **Tree hyperparameters** — Depth, min samples. Lab: tune `max_depth` and observe overfitting.
549. **Random forests** — Bagged trees. Lab: fit a `RandomForestClassifier` and compare to a single tree.
550. **Feature importance** — Tree-based ranking. Lab: extract and plot feature importances.
551. **Gradient boosting** — Sequential boosting. Lab: fit `GradientBoostingClassifier`.
552. **XGBoost** — Optimized boosting. Lab: `pip install xgboost`, train and evaluate a model.
553. **LightGBM** — Fast boosting. Lab: train a LightGBM model and compare speed.
554. **CatBoost** — Categorical boosting. Lab: train CatBoost on data with categorical features.
555. **Support Vector Machines** — Margin maximization. Lab: fit an `SVC` on a 2D dataset.
556. **SVM kernels** — Linear, RBF, poly. Lab: compare decision boundaries across kernels.
557. **Ensemble voting** — Combining models. Lab: build a `VotingClassifier` of three models.
558. **Stacking** — Meta-learning. Lab: build a `StackingClassifier`.
559. **Cross-validation** — Robust evaluation. Lab: run 5-fold CV and report mean/std.
560. **Stratified k-fold** — Balanced folds. Lab: use stratified CV on an imbalanced dataset.
561. **Hyperparameter tuning** — `GridSearchCV`. Lab: grid-search over a model's parameters.
562. **Randomized search** — Efficient tuning. Lab: `RandomizedSearchCV` over a parameter distribution.
563. **Bayesian optimization** — Smart tuning. Lab: tune with `optuna` and compare to grid search.
564. **Pipelines** — Chaining steps. Lab: build a `Pipeline` of scaler + model.
565. **ColumnTransformer** — Per-column preprocessing. Lab: scale numeric and encode categorical columns together.
566. **Feature scaling** — Standardization. Lab: compare model accuracy with and without `StandardScaler`.
567. **Min-max scaling** — Bounded features. Lab: apply `MinMaxScaler` and inspect ranges.
568. **Robust scaling** — Outlier-resistant. Lab: apply `RobustScaler` to skewed data.
569. **One-hot encoding** — Categorical features. Lab: encode categories with `OneHotEncoder` in a pipeline.
570. **Ordinal encoding** — Ordered categories. Lab: encode education levels ordinally.
571. **Target encoding** — Mean encoding. Lab: target-encode a high-cardinality feature.
572. **Handling missing values** — `SimpleImputer`. Lab: impute missing values inside a pipeline.
573. **KNN imputation** — Neighbor-based filling. Lab: impute with `KNNImputer` and compare.
574. **Feature engineering** — Creating predictive features. Lab: build interaction and ratio features.
575. **Datetime features** — Extracting signal from dates. Lab: derive day-of-week and month features.
576. **Binning features** — Discretization. Lab: bin a continuous feature with `KBinsDiscretizer`.
577. **Feature selection (filter)** — Univariate selection. Lab: select top-k features with `SelectKBest`.
578. **Feature selection (wrapper)** — Recursive elimination. Lab: run `RFE` to pick features.
579. **Feature selection (embedded)** — Model-based. Lab: select features via Lasso coefficients.
580. **Handling imbalanced data** — Class weights. Lab: set `class_weight='balanced'` and compare recall.
581. **SMOTE** — Synthetic oversampling. Lab: `pip install imbalanced-learn`, apply SMOTE.
582. **Undersampling** — Reducing majority. Lab: random-undersample and compare metrics.
583. **Threshold tuning** — Adjusting decision cutoff. Lab: pick a threshold optimizing recall.
584. **Calibration** — Reliable probabilities. Lab: calibrate a classifier and plot a reliability curve.
585. **Learning curves** — Data-size effects. Lab: plot a learning curve to diagnose bias/variance.
586. **Validation curves** — Hyperparameter effects. Lab: plot a validation curve over a parameter.
587. **Bias–variance tradeoff** — Model complexity. Lab: demonstrate the tradeoff with a complexity sweep.
588. **Regularization strength** — Controlling complexity. Lab: sweep `C` in logistic regression.
589. **Multiclass strategies** — OvR vs OvO. Lab: classify a 3-class problem and inspect the strategy.
590. **Multilabel classification** — Multiple labels per sample. Lab: fit a multilabel classifier.
591. **k-Means clustering** — Partitioning data. Lab: cluster 2D data and plot the centroids.
592. **Choosing k** — Elbow method. Lab: plot inertia vs k to pick the elbow.
593. **Silhouette score** — Cluster quality. Lab: compute silhouette scores across k values.
594. **Hierarchical clustering** — Dendrograms. Lab: build and plot a dendrogram.
595. **DBSCAN** — Density-based clustering. Lab: cluster non-spherical data with DBSCAN.
596. **Gaussian Mixture Models** — Soft clustering. Lab: fit a GMM and plot probability contours.
597. **PCA** — Dimensionality reduction. Lab: reduce features to 2D and plot.
598. **Explained variance** — PCA component selection. Lab: plot cumulative explained variance.
599. **t-SNE** — Nonlinear embedding. Lab: visualize high-dim data in 2D with t-SNE.
600. **UMAP** — Fast embeddings. Lab: `pip install umap-learn`, embed and plot a dataset.
601. **Anomaly detection** — Isolation Forest. Lab: detect outliers with `IsolationForest`.
602. **One-class SVM** — Novelty detection. Lab: flag anomalies with a one-class SVM.
603. **Association rules** — Market basket analysis. Lab: mine frequent itemsets with `mlxtend`.
604. **Recommendation basics** — Collaborative filtering. Lab: build a simple user-item similarity recommender.
605. **Time-series forecasting (classical)** — ARIMA. Lab: fit an ARIMA model with `statsmodels`.
606. **Seasonal decomposition** — Trend/seasonality. Lab: decompose a time series into components.
607. **Exponential smoothing** — Holt-Winters. Lab: forecast with `ExponentialSmoothing`.
608. **Prophet** — Automated forecasting. Lab: `pip install prophet`, forecast a daily series.
609. **Feature stores concept** — Reusable features. Lab: write notes on why feature stores exist.
610. **Model persistence** — `joblib`. Lab: save and reload a trained model with `joblib.dump`.
611. **Model versioning** — Tracking models. Lab: save models with version tags in filenames.
612. **Reproducible ML** — Seeds & configs. Lab: fix all seeds and reproduce identical results.
613. **Data leakage in pipelines** — Fitting on test data. Lab: reproduce leakage, then fix with a pipeline.
614. **Evaluation on imbalanced data** — Beyond accuracy. Lab: compare accuracy vs F1 on skewed data.
615. **Nested cross-validation** — Unbiased tuning. Lab: run nested CV for honest performance estimates.
616. **Model interpretability: coefficients** — Linear model explanations. Lab: rank features by standardized coefficients.
617. **Permutation importance** — Model-agnostic importance. Lab: compute permutation importance.
618. **Partial dependence plots** — Feature effects. Lab: plot PDP for a top feature.
619. **SHAP values** — Explaining predictions. Lab: `pip install shap`, explain a single prediction.
620. **LIME** — Local explanations. Lab: explain one prediction with LIME.
621. **Fairness basics** — Bias across groups. Lab: compare model metrics across a sensitive group.
622. **Error analysis** — Studying mistakes. Lab: inspect the worst misclassified examples.
623. **Baseline models** — Dummy classifiers. Lab: compare your model against `DummyClassifier`.
624. **Metric selection** — Matching metric to goal. Lab: choose and justify a metric for a business case.
625. **Threshold vs cost** — Business-aware decisions. Lab: pick a threshold minimizing a cost function.
626. **Model cards** — Documenting models. Lab: write a model card for a trained model.
627. **AutoML intro** — Automated modeling. Lab: run `TPOT` or `FLAML` on a dataset.
628. **Handling large datasets** — Incremental learning. Lab: train with `partial_fit` on batches.
629. **Sparse data** — Efficient representations. Lab: train on a sparse matrix from text data.
630. **Text vectorization** — Bag of words. Lab: `CountVectorizer` on a text corpus.
631. **TF-IDF** — Weighted term features. Lab: `TfidfVectorizer` and train a classifier.
632. **N-grams** — Phrase features. Lab: add bigrams to a text classifier.
633. **Text classification** — Spam detection. Lab: build a spam classifier with TF-IDF + Naive Bayes.
634. **Sentiment (classical)** — Polarity classification. Lab: classify review sentiment with logistic regression.
635. **Pipeline for text** — End-to-end NLP pipeline. Lab: build vectorizer + model in one pipeline.
636. **Regression on real data** — Housing prices. Lab: predict prices on a public housing dataset.
637. **Classification on real data** — Churn prediction. Lab: predict customer churn end-to-end.
638. **Clustering on real data** — Customer segmentation. Lab: segment customers with k-Means.
639. **Comparing models systematically** — Benchmark table. Lab: benchmark 5 models on one dataset.
640. **Ensemble of best models** — Combining strengths. Lab: stack your top models for a final score.
641. **Cross-validation strategies for time series** — No shuffling. Lab: use `TimeSeriesSplit`.
642. **Grouped cross-validation** — Avoiding group leakage. Lab: use `GroupKFold` on grouped data.
643. **Handling categorical + numeric together** — Mixed pipelines. Lab: build a full mixed-type pipeline.
644. **Custom transformers** — `BaseEstimator`/`TransformerMixin`. Lab: write a custom feature transformer.
645. **Custom scorers** — Domain metrics. Lab: define a custom scorer for `GridSearchCV`.
646. **Probabilistic outputs** — `predict_proba`. Lab: use probabilities for ranked decisions.
647. **Multi-output regression** — Predicting several targets. Lab: predict two targets at once.
648. **Quantile regression** — Prediction intervals. Lab: predict 10th/90th percentiles.
649. **Survival analysis intro** — Time-to-event. Lab: fit a Kaplan-Meier curve with `lifelines`.
650. **Recommender evaluation** — Ranking metrics. Lab: compute precision@k for recommendations.
651. **Cold-start problem** — New users/items. Lab: write notes and a content-based fallback.
652. **Feature drift** — Distribution shifts. Lab: compare feature distributions across two time periods.
653. **Concept drift** — Changing relationships. Lab: simulate drift and measure accuracy decay.
654. **Model monitoring metrics** — Production signals. Lab: log prediction distributions over time.
655. **Retraining strategy** — When to retrain. Lab: define a retraining trigger rule.
656. **Cost-sensitive learning** — Weighted errors. Lab: apply per-class costs to a classifier.
657. **Semi-supervised learning** — Using unlabeled data. Lab: label-propagate on partially labeled data.
658. **Active learning intro** — Querying informative samples. Lab: pick the most uncertain samples to label.
659. **ML project checklist** — Systematic process. Lab: write a reusable project checklist.
660. **Mini project: Kaggle-style competition** — Full pipeline. Lab: enter a Kaggle competition and submit predictions.

## Phase 9 — Deep Learning Foundations (661–760)

661. **What is deep learning** — Neural networks vs classical ML. Lab: write notes on when DL beats classical ML.
662. **The perceptron** — Single neuron. Lab: implement a perceptron in NumPy for AND/OR.
663. **Activation functions** — Nonlinearity. Lab: plot sigmoid, tanh, and ReLU.
664. **Feedforward networks** — Layers of neurons. Lab: build a 2-layer network in NumPy.
665. **Forward propagation** — Computing outputs. Lab: implement forward pass by hand.
666. **Loss functions** — Measuring error. Lab: implement MSE and cross-entropy in NumPy.
667. **Backpropagation** — Gradient computation. Lab: derive and code backprop for a 1-hidden-layer net.
668. **Gradient descent variants** — SGD, momentum. Lab: implement SGD with momentum manually.
669. **Learning rate scheduling** — Decaying steps. Lab: apply step decay in a manual training loop.
670. **Weight initialization** — Xavier/He. Lab: compare training with zero vs He initialization.
671. **Vanishing gradients** — Deep network problem. Lab: observe shrinking gradients in a deep sigmoid net.
672. **PyTorch intro** — The DL framework. Lab: `pip install torch`, create a tensor, print it.
673. **Tensors** — GPU-ready arrays. Lab: create tensors and move one to GPU if available.
674. **Tensor operations** — Math on tensors. Lab: do matrix multiply and broadcasting with tensors.
675. **Autograd** — Automatic differentiation. Lab: compute gradients with `.backward()`.
676. **Building an `nn.Module`** — Model definition. Lab: define a small feedforward `nn.Module`.
677. **Optimizers** — `torch.optim`. Lab: train a model with the Adam optimizer.
678. **Training loop** — Forward/backward/step. Lab: write a full PyTorch training loop.
679. **DataLoaders** — Batching data. Lab: wrap a dataset in a `DataLoader`.
680. **Custom Datasets** — `Dataset` subclass. Lab: build a custom `Dataset` for CSV data.
681. **Train/val/test in PyTorch** — Proper splits. Lab: evaluate on a validation set each epoch.
682. **Regression with a neural net** — Continuous output. Lab: fit a NN to a noisy sine curve.
683. **Classification with a neural net** — Softmax output. Lab: classify Iris with a PyTorch net.
684. **Overfitting in DL** — Train/val gap. Lab: plot train vs val loss and spot overfitting.
685. **Dropout** — Regularization. Lab: add dropout and compare val loss.
686. **Batch normalization** — Stabilizing training. Lab: add batchnorm and observe faster convergence.
687. **Weight decay** — L2 in optimizers. Lab: add weight decay to Adam.
688. **Early stopping** — Halting on plateau. Lab: implement early stopping on val loss.
689. **Learning rate finder** — Choosing LR. Lab: sweep LRs and plot loss vs LR.
690. **Schedulers in PyTorch** — `lr_scheduler`. Lab: apply cosine annealing.
691. **GPU training** — CUDA tensors. Lab: move model + data to GPU and time an epoch.
692. **Mixed precision** — `torch.cuda.amp`. Lab: train with autocast and compare speed.
693. **Saving/loading models** — `state_dict`. Lab: save and reload model weights.
694. **Reproducibility in DL** — Seeds & determinism. Lab: set all seeds for a repeatable run.
695. **TensorBoard** — Training visualization. Lab: log loss curves to TensorBoard.
696. **Keras/TensorFlow intro** — Alternative framework. Lab: build the same net in Keras `Sequential`.
697. **Keras training** — `compile`/`fit`. Lab: train and evaluate a Keras model.
698. **Framework comparison** — PyTorch vs TF. Lab: note tradeoffs after building in both.
699. **Convolutional layers** — Spatial features. Lab: apply a `Conv2d` to an image tensor.
700. **Pooling layers** — Downsampling. Lab: add max pooling and inspect output shape.
701. **Building a CNN** — Image classifier. Lab: build a CNN for MNIST digits.
702. **Training a CNN** — Full loop. Lab: train the MNIST CNN to >98% accuracy.
703. **Data augmentation** — Synthetic variety. Lab: add random flips/rotations to training images.
704. **Transfer learning** — Pretrained backbones. Lab: fine-tune a pretrained ResNet on a small dataset.
705. **Feature extraction** — Frozen backbones. Lab: use a frozen CNN as a feature extractor.
706. **Fine-tuning strategies** — Unfreezing layers. Lab: gradually unfreeze layers and compare.
707. **CNN architectures** — LeNet, VGG, ResNet. Lab: load and inspect a torchvision ResNet.
708. **Residual connections** — Skip connections. Lab: build a small residual block.
709. **Image classification project** — Real dataset. Lab: classify CIFAR-10 with a CNN.
710. **Recurrent networks (RNN)** — Sequence modeling. Lab: build an RNN for a toy sequence task.
711. **LSTM** — Long-term memory. Lab: build an LSTM for character prediction.
712. **GRU** — Efficient recurrence. Lab: swap LSTM for GRU and compare.
713. **Sequence batching** — Padding & packing. Lab: pad variable-length sequences in a batch.
714. **Text classification with RNN** — Sequential text. Lab: classify sentiment with an LSTM.
715. **Time-series with LSTM** — Forecasting. Lab: forecast a univariate series with an LSTM.
716. **Embeddings** — Learned representations. Lab: add an `nn.Embedding` layer for tokens.
717. **Word embeddings** — Word2Vec/GloVe. Lab: load pretrained GloVe vectors and find nearest words.
718. **Attention mechanism** — Weighted context. Lab: implement scaled dot-product attention in NumPy.
719. **Self-attention** — Sequence-to-sequence context. Lab: code a minimal self-attention block in PyTorch.
720. **The Transformer** — Attention is all you need. Lab: read the architecture and diagram its blocks.
721. **Positional encoding** — Order information. Lab: implement sinusoidal positional encodings.
722. **Multi-head attention** — Parallel attention. Lab: build multi-head attention with `nn.MultiheadAttention`.
723. **Encoder-decoder** — Seq2seq structure. Lab: build a tiny encoder-decoder for reversal.
724. **Building a mini Transformer** — From scratch. Lab: implement a small Transformer block and train on toy data.
725. **Tokenization** — Text to tokens. Lab: tokenize text with `tiktoken` or a BPE tokenizer.
726. **Subword tokenization** — BPE/WordPiece. Lab: train a small BPE tokenizer on a corpus.
727. **Language modeling** — Next-token prediction. Lab: train a char-level language model.
728. **Autoencoders** — Unsupervised compression. Lab: build an autoencoder for MNIST.
729. **Denoising autoencoders** — Robust features. Lab: train an autoencoder to remove noise.
730. **Variational autoencoders** — Generative latent space. Lab: build a VAE and sample new digits.
731. **GAN basics** — Generator vs discriminator. Lab: build a simple GAN on MNIST.
732. **GAN training stability** — Common failures. Lab: observe and mitigate mode collapse.
733. **Conditional GANs** — Class-controlled generation. Lab: generate digits of a chosen class.
734. **Diffusion models (concept)** — Denoising generation. Lab: read the DDPM idea and diagram the forward/reverse process.
735. **Loss landscapes** — Optimization geometry. Lab: visualize a 2D slice of a loss surface.
736. **Gradient clipping** — Exploding gradients. Lab: add gradient clipping to RNN training.
737. **Hyperparameter tuning in DL** — Systematic search. Lab: tune LR and batch size with Optuna.
738. **Model capacity** — Width vs depth. Lab: compare wide vs deep nets on the same data.
739. **Regularization in DL** — Combined techniques. Lab: apply dropout + weight decay + augmentation together.
740. **Class imbalance in DL** — Weighted losses. Lab: apply class weights in the loss function.
741. **Custom loss functions** — Domain-specific losses. Lab: implement a custom PyTorch loss.
742. **Metrics in DL** — Beyond accuracy. Lab: compute F1 during a training loop.
743. **Checkpointing** — Resumable training. Lab: save/restore optimizer + model mid-training.
744. **Multi-GPU concept** — Data parallelism. Lab: read `DataParallel` docs and note requirements.
745. **ONNX export** — Framework-neutral models. Lab: export a PyTorch model to ONNX.
746. **ONNX Runtime** — Fast inference. Lab: run inference on the exported ONNX model.
747. **Quantization** — Smaller, faster models. Lab: dynamically quantize a model and compare size.
748. **Pruning** — Removing weights. Lab: prune a layer and measure accuracy impact.
749. **Knowledge distillation** — Teacher-student. Lab: distill a big model into a smaller one.
750. **Model interpretability in DL** — Saliency maps. Lab: compute a saliency map for an image prediction.
751. **Grad-CAM** — Visual explanations. Lab: generate a Grad-CAM heatmap for a CNN.
752. **Embeddings visualization** — Projecting latents. Lab: project learned embeddings with t-SNE.
753. **Curriculum learning** — Easy-to-hard training. Lab: order training samples by difficulty.
754. **Self-supervised learning** — Learning without labels. Lab: train a contrastive pretext task.
755. **Contrastive learning** — SimCLR-style. Lab: implement a simple contrastive loss.
756. **Meta-learning intro** — Learning to learn. Lab: read few-shot learning basics and summarize.
757. **Reinforcement learning intro** — Agents & rewards. Lab: run a random agent on a Gym environment.
758. **Q-learning** — Value-based RL. Lab: solve FrozenLake with tabular Q-learning.
759. **Deep Q-Networks** — Neural RL. Lab: train a DQN on CartPole.
760. **Mini project: end-to-end DL model** — Train, evaluate, export. Lab: train an image classifier and export it to ONNX with an inference demo.

## Phase 10 — NLP & Large Language Models (761–850)

761. **NLP overview** — Language as data. Lab: write notes mapping NLP tasks to examples.
762. **Text preprocessing** — Cleaning & normalization. Lab: lowercase, strip punctuation, and tokenize text.
763. **Stopwords** — Removing noise words. Lab: filter stopwords with NLTK.
764. **Stemming & lemmatization** — Word normalization. Lab: compare stemmer vs lemmatizer output.
765. **POS tagging** — Grammatical roles. Lab: tag parts of speech with spaCy.
766. **Named entity recognition** — Extracting entities. Lab: extract people/places with spaCy NER.
767. **Dependency parsing** — Sentence structure. Lab: visualize a dependency parse.
768. **Bag of words revisited** — Sparse text features. Lab: build a BoW matrix and inspect vocabulary.
769. **TF-IDF revisited** — Weighted features. Lab: rank the most important terms in documents.
770. **Word2Vec** — Dense word vectors. Lab: train Word2Vec on a corpus with gensim.
771. **Word vector arithmetic** — king − man + woman. Lab: test analogy queries on embeddings.
772. **Document embeddings** — Doc2Vec/averaging. Lab: embed documents by averaging word vectors.
773. **Cosine similarity for text** — Semantic closeness. Lab: find the most similar document to a query.
774. **Topic modeling (LDA)** — Discovering themes. Lab: extract topics from a corpus with `gensim` LDA.
775. **Text classification (modern)** — Neural classifiers. Lab: classify text with an embedding + linear model.
776. **Sequence labeling** — Token-level tasks. Lab: build a simple NER tagger.
777. **HuggingFace intro** — The transformers hub. Lab: `pip install transformers`, load a pipeline.
778. **Using pipelines** — Ready-made NLP. Lab: run sentiment analysis with a `pipeline`.
779. **Pretrained tokenizers** — Model-specific tokenization. Lab: tokenize text with a BERT tokenizer.
780. **BERT** — Bidirectional transformers. Lab: get BERT embeddings for a sentence.
781. **Fine-tuning BERT** — Task adaptation. Lab: fine-tune BERT for text classification.
782. **Sentence transformers** — Semantic embeddings. Lab: `pip install sentence-transformers`, embed sentences.
783. **Semantic search** — Embedding retrieval. Lab: build a semantic search over a document set.
784. **Zero-shot classification** — Label-free classification. Lab: classify text into arbitrary labels zero-shot.
785. **Summarization** — Condensing text. Lab: summarize an article with a transformer pipeline.
786. **Translation** — Cross-language. Lab: translate text with a HuggingFace model.
787. **Question answering** — Extractive QA. Lab: answer questions from a context paragraph.
788. **Text generation** — Causal LMs. Lab: generate text with GPT-2.
789. **Generation parameters** — Temperature, top-k, top-p. Lab: compare outputs across sampling settings.
790. **What is an LLM** — Scale & emergent abilities. Lab: write notes on LLM capabilities and limits.
791. **Transformer decoder** — GPT architecture. Lab: diagram a decoder-only architecture.
792. **Pretraining vs fine-tuning** — Two-stage learning. Lab: summarize the difference with examples.
793. **Prompt engineering** — Crafting inputs. Lab: iterate a prompt to improve an LLM's answer.
794. **Few-shot prompting** — In-context examples. Lab: add examples to a prompt and compare results.
795. **Chain-of-thought** — Reasoning prompts. Lab: prompt step-by-step reasoning on a math problem.
796. **System vs user prompts** — Role structuring. Lab: set a system role and observe behavior changes.
797. **OpenAI/Azure OpenAI API** — Calling hosted LLMs. Lab: call a chat completion from Python.
798. **Token limits & context windows** — Input constraints. Lab: measure token counts with a tokenizer.
799. **Streaming responses** — Incremental output. Lab: stream an LLM response token by token.
800. **Function/tool calling** — Structured actions. Lab: define a tool and let the model call it.
801. **Structured output** — JSON mode/schemas. Lab: force an LLM to return valid JSON.
802. **Embeddings from LLMs** — Vector representations. Lab: generate embeddings via an embeddings API.
803. **Vector databases** — Storing embeddings. Lab: `pip install chromadb`, store and query vectors.
804. **FAISS** — Efficient similarity search. Lab: index embeddings with FAISS and query top-k.
805. **Retrieval-Augmented Generation** — Grounded answers. Lab: build a minimal RAG over your documents.
806. **Chunking strategies** — Splitting documents. Lab: chunk documents with overlap for retrieval.
807. **Re-ranking** — Improving retrieval. Lab: re-rank retrieved chunks with a cross-encoder.
808. **LangChain intro** — LLM orchestration. Lab: `pip install langchain`, run a simple chain.
809. **Prompt templates** — Reusable prompts. Lab: build a parameterized prompt template.
810. **Chains** — Multi-step pipelines. Lab: chain retrieval → prompt → LLM.
811. **Memory in conversations** — Context across turns. Lab: add conversation memory to a chatbot.
812. **LangGraph / agents** — Tool-using LLMs. Lab: build an agent that calls a calculator tool.
813. **ReAct pattern** — Reason + act loops. Lab: implement a reason-then-act agent loop.
814. **LlamaIndex** — Data-framework for LLMs. Lab: build a document index and query it.
815. **Evaluating LLM outputs** — Quality metrics. Lab: score answers with an LLM-as-judge prompt.
816. **Hallucination mitigation** — Grounding techniques. Lab: add citations/grounding to RAG answers.
817. **Guardrails** — Safe outputs. Lab: add input/output validation to an LLM app.
818. **Prompt injection defense** — Security. Lab: test and defend against a prompt-injection attempt.
819. **Cost & latency** — Model economics. Lab: measure tokens, cost, and latency of calls.
820. **Caching LLM responses** — Efficiency. Lab: cache responses to identical prompts.
821. **Fine-tuning LLMs** — Custom behavior. Lab: prepare a small SFT dataset in JSONL.
822. **LoRA / PEFT** — Parameter-efficient tuning. Lab: fine-tune a small model with LoRA.
823. **Quantized LLMs** — Running locally. Lab: run a 4-bit quantized model with `bitsandbytes`.
824. **Local LLMs with Ollama** — On-device inference. Lab: `ollama run` a small model and query it from Python.
825. **Open-source models** — Llama, Mistral, Phi. Lab: load a small open model from HuggingFace.
826. **Instruction tuning** — Following directions. Lab: compare a base vs instruct model on a task.
827. **RLHF concept** — Aligning with preferences. Lab: read RLHF basics and summarize the loop.
828. **DPO concept** — Preference optimization. Lab: prepare a preference-pair dataset format.
829. **Multimodal models** — Text + images. Lab: caption an image with a vision-language model.
830. **Speech-to-text** — Whisper. Lab: transcribe audio with Whisper.
831. **Text-to-speech** — Voice synthesis. Lab: synthesize speech from text with a TTS library.
832. **Document AI** — Extracting from PDFs. Lab: extract structured fields from a PDF.
833. **Agentic workflows** — Multi-step autonomy. Lab: build an agent that plans and executes subtasks.
834. **Multi-agent systems** — Collaborating agents. Lab: build two agents that pass messages.
835. **Tool ecosystems** — Web search, code exec. Lab: give an agent a web-search tool.
836. **Streaming RAG app** — Real-time answers. Lab: build a streaming RAG chatbot UI.
837. **Evaluation datasets for LLMs** — Benchmarks. Lab: evaluate a model on a small QA benchmark.
838. **Prompt versioning** — Managing prompts. Lab: version prompts in files with metadata.
839. **Observability for LLMs** — Tracing calls. Lab: log prompts, responses, and latency to a trace.
840. **Semantic caching** — Embedding-based cache. Lab: cache by semantic similarity of prompts.
841. **Context window management** — Truncation & summarization. Lab: summarize history to fit the window.
842. **Structured RAG** — Metadata filtering. Lab: filter retrieval by document metadata.
843. **Hybrid search** — Keyword + vector. Lab: combine BM25 and vector search results.
844. **Knowledge graphs + LLMs** — Structured grounding. Lab: query a small graph to ground answers.
845. **Safety & moderation** — Content filtering. Lab: run outputs through a moderation check.
846. **Bias in LLMs** — Detecting & reducing. Lab: probe a model for biased completions.
847. **Reproducible LLM apps** — Deterministic configs. Lab: pin temperature/seed and log versions.
848. **Batch LLM processing** — Throughput. Lab: process many prompts efficiently in batches.
849. **Prompt optimization** — Automated improvement. Lab: iterate prompts using an eval loop.
850. **Mini project: production RAG chatbot** — Full stack. Lab: build a RAG chatbot with vector DB, guardrails, and a UI.

## Phase 11 — Computer Vision (851–900)

851. **CV overview** — Images as data. Lab: load and display an image with OpenCV.
852. **Image basics** — Pixels, channels, resolution. Lab: inspect an image's shape and channels.
853. **Color spaces** — RGB, HSV, grayscale. Lab: convert an image between color spaces.
854. **Image resizing** — Scaling & interpolation. Lab: resize an image and compare interpolation methods.
855. **Cropping & rotation** — Geometric transforms. Lab: crop and rotate an image.
856. **Filtering** — Blur, sharpen. Lab: apply Gaussian blur and a sharpen filter.
857. **Edge detection** — Canny/Sobel. Lab: run Canny edge detection on an image.
858. **Thresholding** — Binarization. Lab: apply Otsu thresholding.
859. **Contours** — Shape detection. Lab: find and draw contours of objects.
860. **Morphological ops** — Erosion/dilation. Lab: clean a binary mask with morphology.
861. **Histogram equalization** — Contrast enhancement. Lab: equalize a low-contrast image.
862. **Feature detection** — Corners & keypoints. Lab: detect ORB keypoints in an image.
863. **Feature matching** — Aligning images. Lab: match keypoints between two images.
864. **Image augmentation** — `albumentations`. Lab: build an augmentation pipeline for training.
865. **Datasets & DataLoaders (vision)** — torchvision. Lab: load CIFAR-10 with torchvision.
866. **CNN classifier revisited** — Vision baseline. Lab: train a CNN on a custom image folder.
867. **Transfer learning (vision)** — Pretrained backbones. Lab: fine-tune ResNet on a custom dataset.
868. **Object detection concept** — Boxes & classes. Lab: read YOLO/Faster-RCNN basics and summarize.
869. **Using a pretrained detector** — Inference. Lab: run YOLO on an image and draw boxes.
870. **Training a detector** — Custom objects. Lab: fine-tune a detector on a small labeled set.
871. **Image segmentation concept** — Pixel-level labels. Lab: read semantic vs instance segmentation.
872. **Semantic segmentation** — Pixel classification. Lab: run a pretrained segmentation model.
873. **Instance segmentation** — Mask R-CNN. Lab: run Mask R-CNN and visualize masks.
874. **Pose estimation** — Keypoint detection. Lab: run a pose model on a person image.
875. **Face detection** — Locating faces. Lab: detect faces with a Haar cascade or DNN.
876. **Face recognition** — Identity matching. Lab: compute face embeddings and match identities.
877. **OCR** — Reading text from images. Lab: extract text with Tesseract.
878. **Image similarity** — Embedding-based search. Lab: build reverse image search with embeddings.
879. **Vision transformers (ViT)** — Attention for images. Lab: run a pretrained ViT classifier.
880. **CLIP** — Image-text alignment. Lab: classify images with text prompts using CLIP.
881. **Zero-shot vision** — Prompt-based classification. Lab: classify images into arbitrary categories with CLIP.
882. **Image captioning** — Describing images. Lab: caption images with a vision-language model.
883. **Visual question answering** — Q&A about images. Lab: ask questions about an image.
884. **Image generation** — Diffusion models. Lab: generate an image with Stable Diffusion.
885. **Text-to-image prompting** — Prompt crafting. Lab: iterate prompts to improve generated images.
886. **Image inpainting** — Filling regions. Lab: inpaint a masked region of an image.
887. **Super-resolution** — Upscaling. Lab: upscale a low-res image with a model.
888. **Style transfer** — Artistic rendering. Lab: apply neural style transfer to a photo.
889. **Video basics** — Frames & streams. Lab: read frames from a video with OpenCV.
890. **Video classification** — Temporal models. Lab: classify short clips with a pretrained model.
891. **Object tracking** — Following objects. Lab: track an object across video frames.
892. **Real-time inference** — Webcam pipelines. Lab: run detection on a webcam feed.
893. **Model optimization for vision** — Speed on edge. Lab: quantize a vision model and benchmark.
894. **Deploying vision models** — Serving. Lab: serve an image classifier via an API endpoint.
895. **Annotation tools** — Labeling data. Lab: label a small dataset with a tool like Label Studio.
896. **Data-centric CV** — Improving data quality. Lab: find and fix mislabeled images.
897. **Evaluation metrics (CV)** — mAP, IoU. Lab: compute IoU for predicted vs true boxes.
898. **Handling class imbalance (CV)** — Weighted sampling. Lab: apply weighted sampling to imbalanced classes.
899. **Explainability (CV)** — Grad-CAM revisited. Lab: visualize what a classifier attends to.
900. **Mini project: vision app** — End-to-end. Lab: build an image classification web app with a fine-tuned model.

## Phase 12 — MLOps, Deployment & Production (901–950)

901. **What is MLOps** — ML in production. Lab: diagram the ML lifecycle from data to monitoring.
902. **Model serving concepts** — Batch vs online. Lab: write notes comparing serving modes.
903. **FastAPI intro** — Python web APIs. Lab: `pip install fastapi uvicorn`, build a hello endpoint.
904. **Serving a model** — Prediction endpoint. Lab: wrap a trained model in a FastAPI `/predict`.
905. **Request validation** — Pydantic schemas. Lab: validate input with a Pydantic model.
906. **API testing** — Automated tests. Lab: test the endpoint with `pytest` + `TestClient`.
907. **Dockerizing an ML API** — Containers. Lab: containerize the FastAPI app.
908. **Docker Compose for ML** — Multi-service. Lab: compose API + a vector DB.
909. **Environment configuration** — Settings management. Lab: load config from environment variables.
910. **Model registry** — Tracking versions. Lab: register model versions with MLflow.
911. **Experiment tracking** — MLflow/W&B. Lab: log params/metrics of a training run to MLflow.
912. **Comparing experiments** — Run comparison. Lab: compare multiple runs in the MLflow UI.
913. **Reproducible pipelines** — DVC. Lab: version a dataset and pipeline stage with DVC.
914. **Data versioning** — DVC remotes. Lab: push versioned data to a remote store.
915. **CI/CD for ML** — Automated pipelines. Lab: add a GitHub Action that trains and tests on push.
916. **Model testing** — Behavioral tests. Lab: write invariance and directional tests for a model.
917. **Data validation in production** — Great Expectations. Lab: add data quality checks to a pipeline.
918. **Feature pipelines** — Consistent features. Lab: build a shared feature transform used in train and serve.
919. **Batch inference** — Scheduled scoring. Lab: score a dataset on a schedule with a script.
920. **Streaming inference** — Real-time scoring. Lab: score events from a message queue.
921. **Model monitoring** — Drift & performance. Lab: log prediction distributions and alert on drift.
922. **Logging & observability** — Structured logs. Lab: add structured request/prediction logging.
923. **A/B testing models** — Comparing in production. Lab: route traffic between two model versions.
924. **Canary deployments** — Gradual rollout. Lab: describe and simulate a canary release.
925. **Load testing** — Performance under load. Lab: load-test the API with `locust`.
926. **Autoscaling concept** — Handling demand. Lab: write notes on scaling triggers and strategy.
927. **Caching predictions** — Reducing compute. Lab: cache identical prediction requests.
928. **Model optimization for serving** — ONNX/quantization. Lab: serve an ONNX model and benchmark latency.
929. **GPU serving** — Accelerated inference. Lab: run inference on GPU and compare to CPU.
930. **Serverless ML** — Functions. Lab: deploy a prediction function to a serverless platform.
931. **Kubernetes intro (concept)** — Orchestration. Lab: read pod/deployment/service basics and summarize.
932. **Deploying to Kubernetes** — Manifests. Lab: write a Deployment + Service YAML for the API.
933. **Secrets management** — Secure config. Lab: load secrets from a secret manager, not code.
934. **Security for ML APIs** — Auth & rate limits. Lab: add API key auth and rate limiting.
935. **Input sanitization** — Preventing abuse. Lab: validate and bound all inputs at the API boundary.
936. **Model governance** — Approvals & audit. Lab: write a model approval checklist.
937. **Responsible AI** — Fairness, transparency. Lab: complete a responsible-AI checklist for a model.
938. **Explainability in production** — Serving explanations. Lab: return SHAP-based explanations from the API.
939. **Cost optimization** — Efficient serving. Lab: right-size compute and measure cost per 1k requests.
940. **Pipeline orchestration** — Airflow/Prefect. Lab: build a Prefect flow for train → evaluate → register.
941. **Scheduled retraining** — Automation. Lab: schedule a retraining flow to run weekly.
942. **Shadow deployment** — Risk-free testing. Lab: run a new model in shadow mode logging only.
943. **Rollback strategies** — Safe recovery. Lab: script a rollback to a previous model version.
944. **Model documentation** — Model cards in prod. Lab: publish a model card alongside the deployment.
945. **End-to-end reproducibility** — From data to deploy. Lab: reproduce a deployment from a clean clone.
946. **Monitoring dashboards** — Ops visibility. Lab: build a Grafana/Streamlit dashboard of model metrics.
947. **Alerting** — Proactive ops. Lab: set an alert rule on accuracy drop or latency spike.
948. **Incident response** — ML-specific runbooks. Lab: write a runbook for a model-degradation incident.
949. **Feature/embedding stores in prod** — Serving features. Lab: serve precomputed embeddings from a store.
950. **Mini project: full MLOps pipeline** — Train → serve → monitor. Lab: deploy a model with CI/CD, tracking, an API, and monitoring.

## Phase 13 — Azure AI & Microsoft Foundry (951–1000)

951. **Azure AI landscape** — Services overview. Lab: list relevant Azure AI services and their use cases.
952. **Azure account & CLI** — Tooling setup. Lab: install Azure CLI and run `az login`.
953. **Resource groups** — Organizing resources. Lab: create a resource group with `az group create`.
954. **Azure SDK for Python** — Programmatic access. Lab: `pip install azure-identity`, authenticate with `DefaultAzureCredential`.
955. **Azure Blob Storage** — Cloud data storage. Lab: upload and download a dataset with the storage SDK.
956. **Azure Machine Learning workspace** — ML platform. Lab: create an Azure ML workspace.
957. **Compute in Azure ML** — Training clusters. Lab: create a compute instance/cluster.
958. **Datasets in Azure ML** — Registered data assets. Lab: register a dataset in the workspace.
959. **Training jobs** — Cloud training. Lab: submit a training script as an Azure ML job.
960. **Experiment tracking (Azure ML)** — MLflow integration. Lab: log metrics to Azure ML with MLflow.
961. **Registering models** — Model registry. Lab: register a trained model in Azure ML.
962. **Managed endpoints** — Model deployment. Lab: deploy a model to a managed online endpoint.
963. **Scoring scripts** — Inference entry points. Lab: write a scoring script for the endpoint.
964. **Testing endpoints** — Invoking deployments. Lab: send a test request to the deployed endpoint.
965. **Batch endpoints** — Bulk scoring. Lab: deploy and run a batch scoring endpoint.
966. **Azure AI Services** — Prebuilt AI APIs. Lab: call a prebuilt vision or language API.
967. **Azure AI Language** — Text analytics. Lab: run sentiment and key-phrase extraction via the API.
968. **Azure AI Vision** — Image analysis. Lab: analyze an image with the Vision API.
969. **Azure AI Document Intelligence** — Document extraction. Lab: extract fields from a form/PDF.
970. **Azure AI Speech** — Speech services. Lab: transcribe audio with the Speech SDK.
971. **Azure OpenAI Service** — Hosted LLMs. Lab: deploy a model and call chat completions.
972. **Azure OpenAI embeddings** — Vector generation. Lab: generate embeddings via Azure OpenAI.
973. **Content safety** — Moderation. Lab: run text through Azure AI Content Safety.
974. **Microsoft Foundry overview** — Unified AI platform. Lab: open Foundry and note its core capabilities.
975. **Foundry projects** — Organizing work. Lab: create a Foundry project.
976. **Foundry model catalog** — Choosing models. Lab: browse the catalog and pick a model for a task.
977. **Deploying a model in Foundry** — Serving. Lab: deploy a model from the catalog.
978. **Foundry playground** — Interactive testing. Lab: test prompts in the Foundry playground.
979. **Foundry agents** — Building AI agents. Lab: create a basic Foundry agent.
980. **Adding tools to agents** — Extending capabilities. Lab: add a tool to a Foundry agent.
981. **Agent instructions** — System behavior. Lab: write and refine an agent's instructions.
982. **Knowledge/grounding in Foundry** — RAG on your data. Lab: connect a knowledge source to an agent.
983. **Invoking agents from Python** — Programmatic use. Lab: call a Foundry agent from a Python script.
984. **Foundry evaluations** — Measuring quality. Lab: run a batch evaluation on an agent.
985. **Continuous evaluation** — Ongoing monitoring. Lab: set up continuous evaluation for an agent.
986. **Prompt optimization in Foundry** — Improving prompts. Lab: run the prompt optimizer on an agent.
987. **Tracing in Foundry** — Observability. Lab: enable tracing and inspect agent runs.
988. **Fine-tuning in Foundry** — Custom models. Lab: prepare data and start a fine-tuning job (SFT).
989. **Evaluating fine-tuned models** — Quality checks. Lab: compare base vs fine-tuned model on a test set.
990. **Foundry + azd deployment** — Infra as code. Lab: scaffold and deploy an agent with `azd`.
991. **RBAC & permissions** — Secure access. Lab: assign the needed roles to a Foundry resource.
992. **Managing quotas & capacity** — Scaling. Lab: check model quota and request capacity if needed.
993. **Cost management** — Monitoring spend. Lab: review AI resource costs in the Azure portal.
994. **Responsible AI in Azure** — Safety tooling. Lab: apply content filters and review the RAI dashboard.
995. **Securing AI apps** — Keys & identity. Lab: use managed identity instead of API keys.
996. **Monitoring deployed agents** — Production health. Lab: set up metrics/alerts for a deployed agent.
997. **CI/CD for Foundry agents** — Automated delivery. Lab: add a pipeline that deploys an agent on change.
998. **Multi-agent workflows in Foundry** — Orchestration. Lab: build a workflow coordinating two agents.
999. **End-to-end capstone (cloud)** — Data → model → agent → deploy. Lab: build and deploy a grounded Foundry agent over your own data with evaluation.
1000. **Capstone portfolio & next steps** — Consolidate & showcase. Lab: publish 3 flagship projects (ML, DL/NLP, and a deployed Foundry agent) to GitHub with READMEs, then plan continued specialization.

---

## Suggested Cadence & Milestones

- **Phases 1–3 (Python + tooling):** build fluency; you can script and use Git/VS Code confidently.
- **Phases 4–7 (math + data):** you can wrangle, visualize, and reason about data.
- **Phase 8 (classical ML):** you can frame, train, tune, and evaluate real models.
- **Phase 9 (deep learning):** you can build and train neural networks.
- **Phases 10–11 (NLP/LLMs + CV):** you can build modern AI apps (RAG, vision).
- **Phases 12–13 (MLOps + Azure/Foundry):** you can ship and operate AI in production.

**Habits that make you an expert:** commit every lab to Git, write a one-paragraph summary per phase, rebuild one project from scratch each month, and read one paper/week once you reach Phase 9.
