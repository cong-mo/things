###  String

> Java的String类提供了许多方法来操作字符串。以下是一些常用的String类方法和它们的作用：

1. `length()`: 返回字符串的长度（字符数）。
2. `charAt(int index)`: 返回指定索引位置的字符。
3. `isEmpty()`: 检查字符串是否为空（长度为0）。
4. `equals(Object obj)`: 检查字符串是否与另一个对象相等。
5. `equalsIgnoreCase(String anotherString)`: 检查字符串是否与另一个字符串相等，忽略大小写。
6. `compareTo(String anotherString)`: 按字典顺序比较两个字符串。
7. `concat(String str)`: 将指定字符串连接到当前字符串的末尾。
8. `indexOf(String str)`: 返回第一次出现指定子字符串的索引。
9. `lastIndexOf(String str)`: 返回最后一次出现指定子字符串的索引。
10. `substring(int beginIndex)`: 返回从指定索引开始到字符串末尾的子字符串。
11. `substring(int beginIndex, int endIndex)`: 返回从beginIndex到endIndex之间的子字符串。
12. `startsWith(String prefix)`: 检查字符串是否以指定前缀开头。
13. `endsWith(String suffix)`: 检查字符串是否以指定后缀结尾。
14. `toUpperCase()`: 将字符串中的字符全部转换为大写。
15. `toLowerCase()`: 将字符串中的字符全部转换为小写。
16. `trim()`: 移除字符串两端的空白字符。
17. `replace(char oldChar, char newChar)`: 替换字符串中的指定字符。
18. `replaceAll(String regex, String replacement)`: 使用正则表达式替换字符串中的匹配文本。
19. `split(String regex)`: 使用正则表达式分割字符串并返回一个字符串数组。
20. `contains(CharSequence sequence)`: 检查字符串是否包含指定的字符序列。
21. `charAt(int index)`: 返回指定索引位置的字符。
22. `intern()`: 返回字符串的规范化表示。

> 这些方法允许您在字符串上执行各种操作，如比较、拼接、查找、替换、转换大小写等。根据您的需求，您可以选择适当的方法来操作字符串。



### String Methods

```java
1	public boolean java.lang.String.equals(java.lang.Object)
2	public java.lang.String java.lang.String.toString()
3	public int java.lang.String.hashCode()
4	public int java.lang.String.compareTo(java.lang.Object)
5	public int java.lang.String.compareTo(java.lang.String)
6	public int java.lang.String.indexOf(java.lang.String,int)
7	static int java.lang.String.indexOf(char[],int,int,java.lang.String,int)
8	static int java.lang.String.indexOf(char[],int,int,char[],int,int,int)
9	public int java.lang.String.indexOf(int)
10	public int java.lang.String.indexOf(java.lang.String)
11	public int java.lang.String.indexOf(int,int)
12	public static java.lang.String java.lang.String.valueOf(char)
13	public static java.lang.String java.lang.String.valueOf(java.lang.Object)
14	public static java.lang.String java.lang.String.valueOf(boolean)
15	public static java.lang.String java.lang.String.valueOf(char[],int,int)
16	public static java.lang.String java.lang.String.valueOf(char[])
17	public static java.lang.String java.lang.String.valueOf(double)
18	public static java.lang.String java.lang.String.valueOf(float)
19	public static java.lang.String java.lang.String.valueOf(long)
20	public static java.lang.String java.lang.String.valueOf(int)
21	private static void java.lang.String.checkBounds(byte[],int,int)
22	public int java.lang.String.length()
23	public boolean java.lang.String.isEmpty()
24	public char java.lang.String.charAt(int)
25	public int java.lang.String.codePointAt(int)
26	public int java.lang.String.codePointBefore(int)
27	public int java.lang.String.codePointCount(int,int)
28	public int java.lang.String.offsetByCodePoints(int,int)
29	public void java.lang.String.getChars(int,int,char[],int)
30	void java.lang.String.getChars(char[],int)
31	public byte[] java.lang.String.getBytes()
32	public byte[] java.lang.String.getBytes(java.lang.String) throws java.io.UnsupportedEncodingException
33	public void java.lang.String.getBytes(int,int,byte[],int)
34	public byte[] java.lang.String.getBytes(java.nio.charset.Charset)
35	public boolean java.lang.String.contentEquals(java.lang.StringBuffer)
36	public boolean java.lang.String.contentEquals(java.lang.CharSequence)
37	private boolean java.lang.String.nonSyncContentEquals(java.lang.AbstractStringBuilder)
38	public boolean java.lang.String.equalsIgnoreCase(java.lang.String)
39	public int java.lang.String.compareToIgnoreCase(java.lang.String)
40	public boolean java.lang.String.regionMatches(int,java.lang.String,int,int)
41	public boolean java.lang.String.regionMatches(boolean,int,java.lang.String,int,int)
42	public boolean java.lang.String.startsWith(java.lang.String)
43	public boolean java.lang.String.startsWith(java.lang.String,int)
44	public boolean java.lang.String.endsWith(java.lang.String)
45	private int java.lang.String.indexOfSupplementary(int,int)
46	public int java.lang.String.lastIndexOf(int,int)
47	static int java.lang.String.lastIndexOf(char[],int,int,char[],int,int,int)
48	static int java.lang.String.lastIndexOf(char[],int,int,java.lang.String,int)
49	public int java.lang.String.lastIndexOf(java.lang.String,int)
50	public int java.lang.String.lastIndexOf(int)
51	public int java.lang.String.lastIndexOf(java.lang.String)
52	private int java.lang.String.lastIndexOfSupplementary(int,int)
53	public java.lang.String java.lang.String.substring(int)
54	public java.lang.String java.lang.String.substring(int,int)
55	public java.lang.CharSequence java.lang.String.subSequence(int,int)
56	public java.lang.String java.lang.String.concat(java.lang.String)
57	public java.lang.String java.lang.String.replace(char,char)
58	public java.lang.String java.lang.String.replace(java.lang.CharSequence,java.lang.CharSequence)
59	public boolean java.lang.String.matches(java.lang.String)
60	public boolean java.lang.String.contains(java.lang.CharSequence)
61	public java.lang.String java.lang.String.replaceFirst(java.lang.String,java.lang.String)
62	public java.lang.String java.lang.String.replaceAll(java.lang.String,java.lang.String)
63	public java.lang.String[] java.lang.String.split(java.lang.String,int)
64	public java.lang.String[] java.lang.String.split(java.lang.String)
65	public static java.lang.String java.lang.String.join(java.lang.CharSequence,java.lang.CharSequence[])
66	public static java.lang.String java.lang.String.join(java.lang.CharSequence,java.lang.Iterable)
67	public java.lang.String java.lang.String.toLowerCase(java.util.Locale)
68	public java.lang.String java.lang.String.toLowerCase()
69	public java.lang.String java.lang.String.toUpperCase()
70	public java.lang.String java.lang.String.toUpperCase(java.util.Locale)
71	public java.lang.String java.lang.String.trim()
72	public char[] java.lang.String.toCharArray()
73	public static java.lang.String java.lang.String.format(java.util.Locale,java.lang.String,java.lang.Object[])
74	public static java.lang.String java.lang.String.format(java.lang.String,java.lang.Object[])
75	public static java.lang.String java.lang.String.copyValueOf(char[],int,int)
76	public static java.lang.String java.lang.String.copyValueOf(char[])
77	public native java.lang.String java.lang.String.intern()
```



### 正则表达式

![image-20231019131931124](C:\Users\李Alxe\AppData\Roaming\Typora\typora-user-images\image-20231019131931124.png)





### Collection

集合层次结构中的根接口。集合表示一组对象，称为其元素。某些集合允许重复元素，而其他集合则不允许。有些是有序的，有些是无序的。JDK 不提供此接口的任何直接实现：它提供了更具体的子接口（如 Set 和 List）的实现。此接口通常用于传递集合，并在需要最大通用性的地方操作它们。袋子或多集（可能包含重复元素的无序集合）应直接实现此接口。所有通用 Collection 实现类（通常通过其子接口之一间接实现 Collection）都应提供两个“标准”构造函数：一个 void（无参数）构造函数，用于创建一个空集合，以及一个构造函数，该构造函数具有单个 Collection 类型的参数，该构造函数创建与其参数具有相同元素的新集合。实际上，后一个构造函数允许用户复制任何集合，生成所需实现类型的等效集合。无法强制实施此约定（因为接口不能包含构造函数），但 Java 平台库中的所有通用集合实现都符合此约定。此接口中包含的“破坏性”方法（即修改其操作的集合的方法）被指定为在此集合不支持该操作时引发 UnsupportedOperationException。如果是这种情况，如果调用对集合没有影响，则这些方法可能会（但不是必需）引发 UnsupportedOperationException。例如，在不可修改的集合上调用 addAll（Collection） 方法可能会（但不是必需）在要添加的集合为空时引发异常。某些集合实现对它们可能包含的元素有限制。例如，一些实现禁止空元素，而一些实现对其元素的类型有限制。尝试添加不合格的元素会引发未经检查的异常，通常是 NullPointerException 或 ClassCastException。尝试查询是否存在不符合条件的元素可能会引发异常，或者可能仅返回 false;一些实现将展示前一种行为，而一些实现将展示后者。更一般地说，尝试对不符合条件的元素进行操作，其完成不会导致将不符合条件的元素插入集合中，可能会引发异常，也可能成功，具体取决于实现。此类异常在此接口的规范中标记为“可选”。由每个集合确定自己的同步策略。在实现没有更强的保证的情况下，在集合上调用任何方法可能会导致未定义的行为，该方法正在被另一个线程改变;这包括直接调用、将集合传递给可能执行调用的方法，以及使用现有迭代器检查集合。集合框架接口中的许多方法都是根据 equals 方法定义的。例如，contains（Object o） 方法的规范说：“当且仅当此集合包含至少一个元素 e 时返回 true，使得 （o==null ？e==null ： o.equals（e））.”此规范不应被解释为暗示使用非空参数 o 调用 Collection.contains 将导致对任何元素 e 调用 o.equals（e）。实现可以自由地实现优化，从而避免等于调用，例如，通过首先比较两个元素的哈希码。（Object.hashCode（） 规范保证两个具有不相等哈希码的对象不能相等。更一般地说，各种集合框架接口的实现可以自由地利用基础 Object 方法的指定行为，只要实现者认为合适。某些执行集合递归遍历的集合操作可能会失败，但集合直接或间接包含自身的自引用实例除外。这包括 clone（）、equals（）、hashCode（） 和 toString（） 方法。实现可以选择处理自引用方案，但大多数当前实现不这样做。此接口是 Java 集合框架的成员。



### Collection Methods

```java
public abstract boolean java.util.Collection.add(java.lang.Object)
public abstract boolean java.util.Collection.remove(java.lang.Object)
public abstract boolean java.util.Collection.equals(java.lang.Object)
public abstract int java.util.Collection.hashCode()
public abstract void java.util.Collection.clear()
public abstract boolean java.util.Collection.isEmpty()
public abstract boolean java.util.Collection.contains(java.lang.Object)
public abstract int java.util.Collection.size()
public abstract java.lang.Object[] java.util.Collection.toArray(java.lang.Object[])
public abstract java.lang.Object[] java.util.Collection.toArray()
public abstract java.util.Iterator java.util.Collection.iterator()
public default java.util.Spliterator java.util.Collection.spliterator()
public abstract boolean java.util.Collection.addAll(java.util.Collection)
public default java.util.stream.Stream java.util.Collection.stream()
public abstract boolean java.util.Collection.containsAll(java.util.Collection)
public abstract boolean java.util.Collection.removeAll(java.util.Collection)
public abstract boolean java.util.Collection.retainAll(java.util.Collection)
public default boolean java.util.Collection.removeIf(java.util.function.Predicate)
public default java.util.stream.Stream java.util.Collection.parallelStream()
```





### list

```java
public abstract boolean java.util.List.add(java.lang.Object)
public abstract void java.util.List.add(int,java.lang.Object)
public abstract boolean java.util.List.remove(java.lang.Object)
public abstract java.lang.Object java.util.List.remove(int)
public abstract java.lang.Object java.util.List.get(int)
public abstract boolean java.util.List.equals(java.lang.Object)
public abstract int java.util.List.hashCode()
public abstract int java.util.List.indexOf(java.lang.Object)
public abstract void java.util.List.clear()
public abstract boolean java.util.List.isEmpty()
public abstract int java.util.List.lastIndexOf(java.lang.Object)
public abstract boolean java.util.List.contains(java.lang.Object)
public default void java.util.List.replaceAll(java.util.function.UnaryOperator)
public abstract int java.util.List.size()
public abstract java.util.List java.util.List.subList(int,int)
public abstract java.lang.Object[] java.util.List.toArray()
public abstract java.lang.Object[] java.util.List.toArray(java.lang.Object[])
public abstract java.util.Iterator java.util.List.iterator()
public default java.util.Spliterator java.util.List.spliterator()
public abstract boolean java.util.List.addAll(java.util.Collection)
public abstract boolean java.util.List.addAll(int,java.util.Collection)
public abstract java.lang.Object java.util.List.set(int,java.lang.Object)
public abstract boolean java.util.List.containsAll(java.util.Collection)
public abstract boolean java.util.List.removeAll(java.util.Collection)
public abstract boolean java.util.List.retainAll(java.util.Collection)
public abstract java.util.ListIterator java.util.List.listIterator(int)
public abstract java.util.ListIterator java.util.List.listIterator()
public default void java.util.List.sort(java.util.Comparator)
```





### ArrayList

List 接口的可调整大小数组实现。实现所有可选的列表操作，并允许所有元素，包括 null。除了实现 List 接口之外，此类还提供了操作内部用于存储列表的数组大小的方法。（此类大致等同于 Vector，只是它是不同步的。size、isEmpty、get、set、iterator 和 listIterator 操作在常量时间内运行。添加操作在摊销常量时间内运行，即添加 n 个元素需要 O（n） 时间。所有其他操作都以线性时间运行（粗略地说）。与 LinkedList 实现相比，常量因子较低。每个 ArrayList 实例都有一个容量。容量是用于在列表中存储元素的数组的大小。它始终至少与列表大小一样大。当元素添加到 ArrayList 时，其容量会自动增长。除了添加元素具有恒定的摊销时间成本这一事实之外，没有指定增长策略的详细信息。应用程序可以在使用 ensureCapacity 操作添加大量元素之前增加 ArrayList 实例的容量。这可能会减少增量重新分配的数量。请注意，此实现不同步。如果多个线程同时访问 ArrayList 实例，并且至少有一个线程在结构上修改了该列表，则必须在外部同步该列表。（结构修改是添加或删除一个或多个元素，或显式调整后备数组大小的任何操作;仅设置元素的值不是结构修改。这通常是通过在自然封装列表的某个对象上进行同步来实现的。如果不存在此类对象，则应使用 Collections.syncdList 方法“包装”列表。这最好在创建时完成，以防止意外地不同步访问列表：列表列表 = Collections.syncdList（new ArrayList（...））;此类的迭代器和 listIterator 方法返回的迭代器是快速失败的：如果在创建迭代器后的任何时间对列表进行结构修改，则除了通过迭代器自己的 remove 或 add 方法之外，迭代器将抛出 ConcurrentModificationException。因此，面对并发修改，迭代器会快速而干净地失败，而不是冒着在未来不确定的时间出现任意、非确定性行为的风险。请注意，无法保证迭代器的快速故障行为，因为一般来说，在存在不同步的并发修改的情况下，不可能做出任何硬保证。Fail-fast 迭代器会尽最大努力抛出 ConcurrentModificationException。因此，编写一个依赖于此异常的正确性的程序是错误的：迭代器的快速故障行为应仅用于检测错误。此类是 Java 集合框架的成员。



### File Methods

```java
  1. `public boolean equals(Object obj)`：比较两个文件是否相等。
  2. `public String toString()`：返回文件的字符串表示。
  3. `public int hashCode()`：返回文件的哈希码。
  4. `public int compareTo(Object anotherFile)`：比较两个文件的名称。
  5. `public int compareTo(File anotherFile)`：比较两个文件的名称。
  6. `public String getName()`：返回文件的名称。
  7. `public long length()`：返回文件的大小。
  8. `public String getParent()`：返回文件的父目录。
  9. `public boolean isAbsolute()`：检查文件是否为绝对路径。
  10. `public String getCanonicalPath() throws IOException`：返回文件的规范路径。
  11. `private synchronized void readObject(ObjectInputStream s) throws IOException, ClassNotFoundException`：从输入流中读取对象。
  12. `private synchronized void writeObject(ObjectOutputStream s) throws IOException`：将对象写入输出流。
  13. `public boolean delete()`：删除文件。
  14. `public boolean setReadOnly()`：设置文件为只读。
  15. `public String[] list()`：返回文件的子目录和文件列表。
  16. `public String[] list(FilenameFilter filter)`：返回文件的子目录和文件列表，过滤满足特定条件的文件。
  17. `final boolean isInvalid()`：检查文件是否无效。
  18. `int getPrefixLength()`：返回路径前缀的长度。
  19. `public File getParentFile()`：返回文件的父目录文件。
  20. `public String getPath()`：返回文件的完整路径。
  21. `public String getAbsolutePath()`：返回文件的绝对路径。
  22. `public File getAbsoluteFile()`：返回文件的绝对路径。
  23. `public File getCanonicalFile() throws IOException`：返回文件的规范路径。
  24. `private static String slashify(String path, boolean isAbsolute)`：将路径转换为绝对路径或相对路径。
  25. `public URL toURL() throws MalformedURLException`：返回文件的URL。
  26. `public URI toURI()`：返回文件的URI。
  27. `public boolean canRead()`：检查文件是否可以读取。
  28. `public boolean canWrite()`：检查文件是否可以写入。
  29. `public boolean exists()`：检查文件是否存在。
  30. `public boolean isDirectory()`：检查文件是否为目录。
  31. `public boolean isFile()`：检查文件是否为普通文件。
  32. `public boolean isHidden()`：检查文件是否为隐藏文件。
  33. `public long lastModified()`：返回文件的最后修改时间。
  34. `public boolean createNewFile()` throws IOException：创建新文件。
  35. `public void deleteOnExit()`：在程序退出时删除文件。
  36. `private final String[] normalizedList()`：返回文件的规范列表。
  37. `public File[] listFiles()`：返回文件的子目录和文件列表。
  38. `public File[] listFiles(FileFilter filter)`：返回文件的子目录和文件列表，过滤满足特定条件的文件。
  39. `public File[] listFiles(FilenameFilter filter)`：返回文件的子目录和文件列表，过滤满足特定条件的文件。
  40. `public boolean mkdir()`：创建目录。
  41. `public boolean mkdirs()`：创建目录及其所有父目录。
  42. `public boolean renameTo(File dest)`：将文件重命名为新的文件名。
  43. `public boolean setLastModified(long time)`：设置文件的最后修改时间。
  44. `public boolean setWritable(boolean writable, boolean ownerOnly)`：设置文件的写入权限。
  45. `public boolean setReadable(boolean readable, boolean ownerOnly)`：设置文件的读取权限。
  46. `public boolean setExecutable(boolean executable, boolean ownerOnly)`：设置文件的执行权限。
  47. `public boolean canExecute()`：检查文件是否可以执行。
  48. `public static File[] listRoots()`：返回文件系统的根目录。
  49. `public long getTotalSpace()`：返回文件系统的总空间。
  50. `public long getFreeSpace()`：返回文件系统的可用空间。
  51. `public long getUsableSpace()`：返回文件系统的可使用空间。
  52. `public static File createTempFile(String prefix, String suffix, File directory) throws IOException`：创建一个临时文件。
  53. `public static File createTempFile(String prefix, String suffix) throws IOException`：创建一个临时文件。
  54. `public java.nio.file.Path toPath()`：返回文件的路径。
```

