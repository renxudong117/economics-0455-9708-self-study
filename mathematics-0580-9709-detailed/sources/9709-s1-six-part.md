# Cambridge 9709 S1 Probability & Statistics 1

全册六段式双语学习教材｜2026-2027

## 目录与考纲覆盖

## 单元 1｜5.1 数据的表示｜Representation of data

### 一、单元导读｜Unit introduction

本单元把一组原始数据转化为可以比较、解释和作图的信息。学习顺序是：先分清数据类型和统计量，再学习茎叶图、累计频数图与箱线图，最后处理组距不等的直方图。Paper 5 常把计算与解释放在同一题中，因此答案既要有数值，也要说明这个数值反映了中心位置还是离散程度。

**与国内课程衔接｜Connection with Chinese curriculum.** 与国内初中统计相比，Cambridge 更强调 standard deviation、frequency density、累计频数估计和两组数据的有证据比较。与高中统计衔接时，要特别注意本卷使用的是给定总体公式；分组数据以组中值代替原值，所以所得 mean 和 standard deviation 是 estimates。

**学习路线｜Learning route.** 原始/频数数据 → mean 与 standard deviation → 编码还原 → 有序数据与五数概括 → cumulative frequency → box plot 比较 → histogram 的面积原则。

### 二、知识点精讲｜Detailed teaching

#### 5.1.1 集中趋势、离散程度与编码数据｜Averages, variation and coded data

##### 知识点 01｜均值、中位数、众数与离散程度｜Measures of location and spread

本课研究数据的中心与离散。**mean（均值）**使用全部观测值，**median（中位数）**由排序位置决定，**mode（众数）**是最常出现的值；range、interquartile range 与 standard deviation 则从不同角度描述 spread。离散或连续、原始或分组的数据会影响可用的计算方法和答案是否只是估计。

**English explanation.** The mean is a measure of location and the variance is a measure of spread. A frequency is a weight: each value contributes f times to the totals. Always distinguish variance, measured in squared units, from standard deviation, measured in the original unit.

##### 知识点 02｜原始、频数与编码数据的公式｜Formulae for raw, frequency and coded data

未分组数据：mean = Σx/n。频数表：mean = Σfx/Σf。总体方差为 Var(X)=Σx²/n-(Σx/n)²；频数表对应 Σfx²/Σf-(Σfx/Σf)²。standard deviation 是方差的正平方根。若编码 y=(x-a)/b，则 x=a+by，所以 mean(x)=a+b mean(y)，Var(x)=b²Var(y)。

##### 知识点 03｜方差快捷公式从何而来｜Deriving the variance identity

方差把每个值与均值的离差平方后取平均。平方有两个作用：正负离差不会抵消，而且离均值更远的值被更重地惩罚。快捷公式由展开 (x-mean)² 得到，所以两式计算同一个量。

##### 知识点 04｜从数据表到均值和标准差｜A reliable calculation sequence

写表格列 x、f、fx、fx²。先算 Σf 确认总频数；再算 Σfx 得均值；接着算 Σfx²；最后代入方差公式。若题目给 Σ(x-a) 或 Σ(x-a)²，先在编码变量上计算，再按 x=a+by 还原。不要把 standard deviation 与 variance 混写：前者与原数据同单位，后者是平方单位。

##### 知识点 05｜未分组数据的完整计算｜Worked raw-data calculation

**题目｜Question.** 数据 3,5,5,7,10 的 mean 和 variance。

**正确答案｜Correct answer.** Σx=30，n=5，所以 mean=30/5=6。Σx²=9+25+25+49+100=208。variance=208/5-6²=41.6-36=5.6；sd=√5.6≈2.37。

##### 知识点 06｜用编码总量还原统计量｜Recovering statistics from coded totals

**题目｜Question.** 20 个数据满足 Σ(x-10)=70、Σ(x-10)²=445。求 mean 与 variance。

**正确答案｜Correct answer.** 令 y=x-10。Σy=70，所以 mean(y)=70/20=3.5，mean(x)=13.5。Var(x)=Var(y)=445/20-3.5²=22.25-12.25=10；平移10不改变方差。

##### 知识点 07｜估计值、单位与标准差口径｜Estimation, units and standard-deviation conventions

计算器的 σx 与 sx 可能分别表示总体和样本标准差。Cambridge 题目要求哪一种取决于题设与考纲口径；手算时必须依照给定公式。分组数据只能用组中值估计，因此答案要写 estimated mean。

##### 英文概念串联｜Connected explanation in English

A statistical summary needs both location and spread. The mean uses every observation, so it reacts to an extreme value; the median depends on position and is usually more resistant. Standard deviation measures a typical distance from the mean in the original units, whereas variance is measured in squared units. For grouped data, replace each unknown observation by its class midpoint, so the resulting statistics are estimates.

##### 英文方法说明｜Method in English

For a frequency table, treat frequency as a weight: form fx and fx squared before adding the columns. When coded totals are given, work with the coded variable first and then reverse the transformation. Adding a constant shifts the mean but not the standard deviation; multiplying every value by b multiplies the standard deviation by the absolute value of b and the variance by b squared.

#### 5.1.2 茎叶图、累计频数与箱线图｜Stem-and-leaf, cumulative frequency and box plots

##### 知识点 01｜三种表示分别保留什么信息｜What each representation preserves

**ordered stem-and-leaf diagram**保留每个原始值；**cumulative frequency graph**把“不超过某个上组界”的累计人数画成递增曲线；**box-and-whisker plot**用 minimum、Q1、median、Q3、maximum 概括分布。三种表示承担不同任务，但都要求先明确排序、组界和样本总数。

**English explanation.** A cumulative frequency curve converts ranks into estimated data values. A box plot then compresses the distribution into five summary values. Compare medians for location and IQRs for consistency, quoting values from the common scale.

##### 知识点 02｜从累计频数定位四分位数｜Locating quartiles from cumulative frequency

累计频数逐组相加，横坐标使用 upper class boundary。样本量为 N 时，从累计频数轴读取 N/4、N/2、3N/4 对应的 Q1、median、Q3，并计算 IQR=Q3-Q1。由曲线估计 P(X≤a) 时，用读出的累计频数除以 N。

##### 知识点 03｜画图与读图的完整顺序｜Constructing and reading the diagrams

茎叶图必须按序并写 key，例如 3|7 means 37。累计频数图先算累计列，再以上组界为横坐标作点并平滑连接；读四分位数时从累计频数轴水平到曲线，再垂直到数据轴。箱线图使用同一五数概括，比较两组时必须统一刻度，并分别评论 median 与 IQR。

##### 知识点 04｜由有序数据求五数概括｜Five-number summary from ordered data

**题目｜Question.** 数据 4,7,8,8,10,13,15,19,22，求median、Q1、Q3与IQR。

**正确答案｜Correct answer.** n=9，median为第5个值10。下半4,7,8,8的Q1=(7+8)/2=7.5；上半13,15,19,22的Q3=(15+19)/2=17；IQR=9.5。

##### 知识点 05｜由累计频数读四分位数｜Quartiles from a cumulative-frequency curve

**题目｜Question.** 80 个数据的累计频数图上，CF=20、40、60 对应 x=18、26、35。求 Q1、median、Q3 与 IQR。

**正确答案｜Correct answer.** N/4=20、N/2=40、3N/4=60，所以 Q1=18、median=26、Q3=35，IQR=35-18=17。这些数值由曲线估计，精度应与图上刻度一致。

##### 知识点 06｜比较分布不能只说“更好”｜Making a supported comparison

“A更好”不是统计结论，除非题目定义数值越大或越小代表更好。应该写 higher/lower median 和 more/less consistent，并引用图中数值。两个箱线图必须使用同一刻度才能视觉比较。

##### 英文概念串联｜Connected explanation in English

Choose a representation according to the information that must remain visible. A stem-and-leaf diagram preserves every observation; a cumulative-frequency curve is best for estimating ranks and proportions; a box plot sacrifices detail in order to compare location and spread quickly. A complete comparison quotes numerical evidence rather than relying on the apparent shape alone.

##### 英文方法说明｜Method in English

On a cumulative-frequency graph, plot cumulative totals against upper class boundaries. To estimate a percentile, locate the required cumulative frequency on the vertical axis, move horizontally to the curve and then vertically to the data axis. When comparing box plots, discuss median for location and IQR for consistency, and remember that the word better needs a contextual definition.

#### 5.1.3 直方图与频数密度｜Histograms and frequency density

##### 知识点 01｜面积代表频数｜Area represents frequency

直方图用于连续分组数据。横轴是 class interval，纵轴通常是 **frequency density**；柱子的面积而不是高度代表frequency。柱子相接，因为连续变量在组界之间没有类别空隙。

**English explanation.** In a histogram, area represents frequency. Frequency density corrects for unequal class widths. A taller bar does not necessarily contain more observations; compare areas, not heights, when widths differ.

##### 知识点 02｜频数密度与组距｜Frequency density and class width

frequency density = frequency / class width；因此 frequency = density × class width。若纵轴给的是其他密度标度，仍以面积成比例为原则。组界必须连续，例如10<x≤20与20<x≤35。

##### 知识点 03｜为什么不能把频数直接当柱高｜Why raw frequency is not the height

当组距不相等时，直接用frequency作高度会让宽组获得过大的面积。除以class width后，每个单位宽度承担相同的频数尺度，于是柱面积 width×density 正好恢复frequency。

##### 知识点 04｜从频数表作图和从图反求频数｜Drawing and reversing a histogram

第一步写每组class width；第二步算density；第三步画连续组界；第四步标纵轴。反向读图时先读高度，再乘组距求frequency。求某个子区间人数时按同一柱内均匀分布作比例估计。

##### 知识点 05｜不等组距的柱高计算｜Unequal-width class calculation

**题目｜Question.** 区间0≤t<5频数20；5≤t<15频数30。求两柱高度。

**正确答案｜Correct answer.** 第一组宽5，density=20/5=4。第二组宽10，density=30/10=3。虽然第二组频数更大，柱高反而较低，因为柱更宽。

##### 知识点 06｜柱内子区间的频数估计｜Estimating a sub-interval frequency

**题目｜Question.** 20≤x<30的柱高2.4；估计22≤x<27的频数。

**正确答案｜Correct answer.** 整组密度2.4，子区间宽5，所以估计频数=2.4×5=12。这里使用组内均匀分布假设。

##### 知识点 07｜直方图与条形图的边界｜Histogram versus bar chart

bar chart与histogram不同：bar chart处理类别/离散值，柱间可留空，高度通常表示频数；histogram处理连续分组数据，柱相接，面积表示频数。不要使用组中值画直方图。

##### 英文概念串联｜Connected explanation in English

A histogram is an area diagram. The width of a bar is the class width and the height is frequency density, so area equals class width multiplied by frequency density and is proportional to frequency. This convention prevents a wide class from looking artificially important merely because it covers a larger interval.

##### 英文方法说明｜Method in English

Begin by writing the continuous class boundaries and calculating every class width. Then divide frequency by width to obtain each height. When reading a histogram in reverse, multiply height by width. If only part of a bar is required, the calculation assumes that observations are spread uniformly within that class; state this assumption when the question asks for an estimate.

### 三、核心词汇表｜Core vocabulary

- **raw data**｜原始数据：observations before they are grouped or summarised
- **discrete data**｜离散数据：data obtained by counting, with separate possible values
- **continuous data**｜连续数据：measurements that may take any value in an interval
- **frequency**｜频数：the number of observations having a value or lying in a class
- **class interval**｜组距区间：a stated interval used to group continuous data
- **class width**｜组宽：upper class boundary minus lower class boundary
- **class midpoint**｜组中值：the average of the two class boundaries
- **mean**｜均值：the total of the values divided by their number
- **median**｜中位数：the middle value or central pair after ordering
- **mode**｜众数：the value occurring most often
- **range**｜极差：maximum minus minimum
- **quartile**｜四分位数：a value dividing ordered data into quarters
- **interquartile range**｜四分位距：Q3 minus Q1, measuring the middle 50% spread
- **variance**｜方差：the mean squared deviation from the mean
- **standard deviation**｜标准差：the positive square root of variance
- **coded data**｜编码数据：data transformed to simplify arithmetic
- **estimated mean**｜估计均值：a mean found using class midpoints in place of raw values
- **stem-and-leaf diagram**｜茎叶图：an ordered display that retains every original value
- **back-to-back stem-and-leaf**｜背靠背茎叶图：two stem-and-leaf displays sharing stems
- **key**｜图键：a statement explaining how a stem and leaf form a value
- **cumulative frequency**｜累计频数：the number of observations up to a boundary
- **upper class boundary**｜上组界：the right-hand endpoint plotted on a cumulative-frequency graph
- **percentile**｜百分位数：a value below which a stated percentage lies
- **box-and-whisker plot**｜箱线图：a display of the five-number summary
- **frequency density**｜频数密度：frequency divided by class width
- **histogram**｜直方图：a continuous grouped-data graph whose bar area represents frequency
- **bar chart**｜条形图：a category display whose separated bar heights represent values
- **outlier**｜异常值：an observation unusually far from the main body of data
- **location**｜位置：the central or typical level of a distribution
- **spread**｜离散程度：the amount by which observations vary

### 四、单元练习｜Unit practice（共 21 题）

#### 1.1 辨认连续数据｜Identifying continuous data

A delivery company records waiting times of 4.2, 5.7 and 6.1 minutes. State the type of data and explain why.

#### 1.2 由频数表计算方差｜Variance from a frequency table

The values 2,4,6 have frequencies 1,3,2. Find the variance.

#### 1.3 分组数据为何只能估计｜Why grouped results are estimates

A student uses class midpoints to calculate a mean of 27.4 and writes “the mean is exactly 27.4”. Correct the conclusion.

#### 1.4 线性变换怎样改变统计量｜Effect of a linear transformation

Every value in a data set is transformed by y=3x-2. How do mean and variance change?

#### 1.5 选择与辨析｜Multiple choice

For values 1,2,4 with frequencies 3,2,1, what is the mean?
A 1.5  B 2.0  C 11/6  D 7/3

#### 1.6 综合应用 2｜Extended application 2

For the data 2, 4, 4, 6, derive the variance using both forms of the formula.

#### 1.7 综合应用 4｜Extended application 4

A set has mean 12 and variance 9. Every value is changed by y=2x+5. Explain in English how the two statistics change.

#### 1.8 从有序数据求四分位数｜Quartiles from ordered data

The ordered data are 6, 8, 9, 12, 14, 18, 21, 25. Find the median, Q1, Q3 and IQR.

#### 1.9 用中位数和 IQR 比较两组｜Comparing two distributions

Explain how to compare two distributions using box plots.

#### 1.10 订正没有语境的“更好”｜Correcting an unsupported comparison

A student says “Group A is better because its box is shorter.” Group A has median 72 and IQR 6; Group B has median 65 and IQR 11. Rewrite the comparison accurately.

#### 1.11 选择与辨析｜Multiple choice

Which statistic is least affected by one extremely large value?
A mean  B range  C median  D standard deviation

#### 1.12 迁移应用｜Transfer problem

If 5 is added to every observation, what happens to median and IQR?

#### 1.13 综合应用 2｜Extended application 2

Explain why the IQR is often preferred to the range when a distribution contains an extreme value.

#### 1.14 综合应用 4｜Extended application 4

Two box plots show delivery times. A has median 18 minutes and IQR 5 minutes; B has median 15 minutes and IQR 12 minutes. Compare them in English.

#### 1.15 不等组距的频数密度｜Frequency density with unequal widths

A class 10≤x<18 has frequency 24 and a class 18≤x<30 has frequency 30. Calculate both bar heights.

#### 1.16 由柱高反求频数｜Recovering frequency from a bar

A histogram bar covers 40≤x<55 and has density 3.2. Find its frequency.

#### 1.17 订正把频数当柱高的错图｜Correcting histogram heights

A student draws heights 20 and 30 for classes of widths 5 and 15 because those are their frequencies. Explain and repair the error.

#### 1.18 选择与辨析｜Multiple choice

A class has width 8 and frequency 36. What is its frequency density?
A 4  B 4.5  C 28  D 288

#### 1.19 迁移应用｜Transfer problem

Two bars have equal height but widths 5 and 12. Compare frequencies.

#### 1.20 综合应用 2｜Extended application 2

Derive the formula frequency = class width × frequency density from the meaning of histogram area.

#### 1.21 综合应用 4｜Extended application 4

One histogram bar covers 40≤t<60 at density 2.5. Estimate the number with 48≤t<56 and explain the assumption.

### 五、练习答案与解析｜Answers and explanations（共 21 题）

#### 1.1 辨认连续数据｜Identifying continuous data

**完整解答｜Full solution.** Waiting time is **continuous data**. Time can, in principle, take any value in an interval; 4.2 minutes is rounded from a measurement rather than obtained by counting. It is therefore not discrete simply because the recorded values have one decimal place.

#### 1.2 由频数表计算方差｜Variance from a frequency table

**完整解答｜Full solution.** Σf=6, Σfx=26, so mean=13/3. Σfx²=4+48+72=124. Variance=124/6-(13/3)²=35/18≈1.94.

#### 1.3 分组数据为何只能估计｜Why grouped results are estimates

**完整解答｜Full solution.** The value is an **estimated mean**, not an exact mean. Every observation in a class has been represented by its midpoint, although the original values may lie anywhere within that class. The corrected conclusion is: “The estimated mean is 27.4.”

#### 1.4 线性变换怎样改变统计量｜Effect of a linear transformation

**完整解答｜Full solution.** E(Y)=3E(X)-2. Var(Y)=3²Var(X)=9Var(X); subtracting 2 changes location but not spread.

#### 1.5 选择与辨析｜Multiple choice

**完整解答｜Full solution.** C - 11/6. Σfx=3+4+4=11 and Σf=6, so mean=11/6.

#### 1.6 综合应用 2｜Extended application 2

**完整解答｜Full solution.** **第 1 步｜Step 1.** Mean = Σx/n = 16/4 = 4.  **第 2 步｜Step 2.** Direct form: Σ(x−4)²/4 = (4+0+0+4)/4 = 2.  **第 3 步｜Step 3.** Shortcut form: Σx²/n−x̄² = (4+16+16+36)/4−4² = 72/4−16 = 2. Both forms agree because expanding Σ(x−x̄)² produces Σx²−nx̄².

#### 1.7 综合应用 4｜Extended application 4

**完整解答｜Full solution.** Adding 5 shifts every observation equally, so it raises the mean but does not change the spread. Multiplying by 2 doubles every deviation from the mean, so the variance is multiplied by 2². Hence E(Y)=2(12)+5=29 and Var(Y)=4(9)=36.

#### 1.8 从有序数据求四分位数｜Quartiles from ordered data

**完整解答｜Full solution.** There are 8 values. **Median** = (12+14)/2 = 13. The lower half is 6,8,9,12, so **Q1**=(8+9)/2=8.5. The upper half is 14,18,21,25, so **Q3**=(18+21)/2=19.5. Therefore **IQR**=19.5−8.5=11.

#### 1.9 用中位数和 IQR 比较两组｜Comparing two distributions

**完整解答｜Full solution.** Compare medians for location and compare IQRs (or ranges) for spread. Quote both pairs of values and interpret in context; do not infer causation.

#### 1.10 订正没有语境的“更好”｜Correcting an unsupported comparison

**完整解答｜Full solution.** A shorter box shows a smaller IQR, not automatically a “better” group. The supported statement is: **Group A has a higher median (72 compared with 65) and is more consistent because its IQR is smaller (6 compared with 11).** Whether a higher value is better depends on the context.

#### 1.11 选择与辨析｜Multiple choice

**完整解答｜Full solution.** C - median. Its position in the ordered list may be unchanged, while the mean, range and standard deviation respond to the extreme value.

#### 1.12 迁移应用｜Transfer problem

**完整解答｜Full solution.** Median increases by 5. Both Q1 and Q3 increase by 5, so IQR=(Q3+5)-(Q1+5) is unchanged.

#### 1.13 综合应用 2｜Extended application 2

**完整解答｜Full solution.** Range uses only maximum−minimum, so one extreme observation can alter it greatly. IQR=Q3−Q1 uses the middle 50% of ordered observations. An extreme maximum may leave Q1 and Q3 unchanged, so the IQR gives a more resistant measure of spread.

#### 1.14 综合应用 4｜Extended application 4

**完整解答｜Full solution.** Company B is typically faster because its median delivery time is lower, 15 minutes rather than 18 minutes. However, company A is more consistent because its interquartile range is smaller, 5 minutes rather than 12 minutes.

#### 1.15 不等组距的频数密度｜Frequency density with unequal widths

**完整解答｜Full solution.** First class width=18−10=8, so density=24/8=3. Second class width=30−18=12, so density=30/12=2.5. The first bar is taller even though its frequency is smaller, because histogram height is **frequency per unit width**.

#### 1.16 由柱高反求频数｜Recovering frequency from a bar

**完整解答｜Full solution.** Class width=15. Frequency=3.2×15=48.

#### 1.17 订正把频数当柱高的错图｜Correcting histogram heights

**完整解答｜Full solution.** Unequal widths make raw frequency an invalid height. Correct densities are 20/5=4 and 30/15=2. Thus the first bar must be twice as tall as the second. Their areas are 5×4=20 and 15×2=30, which recover the stated frequencies.

#### 1.18 选择与辨析｜Multiple choice

**完整解答｜Full solution.** B - 4.5, because 36/8=4.5.

#### 1.19 迁移应用｜Transfer problem

**完整解答｜Full solution.** They have the same density, so frequencies are proportional to widths. The second frequency is 12/5 times the first.

#### 1.20 综合应用 2｜Extended application 2

**完整解答｜Full solution.** In a histogram, **bar area represents frequency**. Rectangle area = width×height. Here width is class width and height is frequency density, so frequency = class width×frequency density. Rearranging gives density=frequency/class width.

#### 1.21 综合应用 4｜Extended application 4

**完整解答｜Full solution.** The required subinterval has width 56−48=8, so the estimated frequency is 8×2.5=20. This assumes observations are distributed uniformly within the class interval.

### 六、自学检查清单｜Self-study checklist

- [ ] I can distinguish discrete from continuous data from the method of collection.
- [ ] I can calculate mean and standard deviation from raw data, a frequency table or supplied totals.
- [ ] I can reverse a linear code and explain why adding a constant does not change spread.
- [ ] I can construct and interpret ordered and back-to-back stem-and-leaf diagrams with a key.
- [ ] I can use upper class boundaries on a cumulative-frequency graph.
- [ ] I can estimate quartiles, percentiles and proportions from a cumulative-frequency graph.
- [ ] I can compare two data sets using quoted medians and IQRs or standard deviations.
- [ ] I can calculate frequency density and explain why histogram area represents frequency.
- [ ] I can distinguish a histogram from a bar chart and avoid using raw frequency as height for unequal widths.

## 单元 2｜5.2 排列与组合｜Permutations and combinations

### 一、单元导读｜Unit introduction

本单元研究有限步骤共有多少种结果。关键不是按计算器，而是判断交换两个已选对象会不会得到新结果。若顺序、职位、座位或密码位置不同会产生新结果，用 permutation；若只是组成一个没有职位差别的小组，用 combination。限制条件要先翻译，再决定分情况、捆绑或补集。

**与国内课程衔接｜Connection with Chinese curriculum.** 国内课程常把排列与组合直接写成公式。本单元进一步要求把公式还原为乘法原理，并用英文识别 arrange、select、at least、together、not next to 等限制词。圆排列不在 9709 S1 范围内。

**学习路线｜Learning route.** 乘法原理 → factorial → nPr → 重复对象和相邻限制 → nCr 的来源 → exactly/at least/at most → 分步选择与分配。

### 二、知识点精讲｜Detailed teaching

#### 5.2.1 排列：顺序为什么重要｜Permutations and factorial notation

##### 知识点 01｜交换后是否成为新结果｜The order test for permutations

**排列（permutation）**解决“选出后还要安排顺序”的问题。若从n个不同对象中依次取r个，顺序不同算不同结果，数量为 nPr=n!/(n-r)!。n!=n(n-1)...2×1，且0!=1。

**English explanation.** Use a permutation when order creates a different outcome. The formula nPr is a compact form of the product n(n-1)... . For repeated objects, divide by the factorial of each repetition because swaps within identical objects have been overcounted.

##### 知识点 02｜阶乘与 nPr 的逐位置含义｜Factorials and the factors in nPr

nPr可展开为 n(n-1)...(n-r+1)。例如8P3=8×7×6=336：第一个位置8种，选定后第二个7种，第三个6种。这个乘法过程就是公式的来源，不是需要死背的符号。

##### 知识点 03｜从乘法原理推出排列公式｜Deriving nPr from the product rule

乘法原理说明：若第一步有a种、每种情况下第二步有b种，则有ab种有序结果。8人选主席、秘书、财务员时三个职位不同，所以A任主席B任秘书与B任主席A任秘书是不同安排。

##### 知识点 04｜限制条件先处理哪个位置｜Handling restricted positions

看到题目先问：是否有位置、次序、排名、座位或密码？若交换两个已选对象会产生新结果，就用排列。然后逐位置写可选数，比直接按 nPr 更能防止限制条件出错。

##### 知识点 05｜不同职位的安排｜Allocating distinct offices

**题目｜Question.** 8个人中选主席、秘书、财务员，各职位一人，有多少种？

**正确答案｜Correct answer.** 职位不同，顺序重要。第一职8选1，第二职剩7人，第三职剩6人：8×7×6=336。也可写 8P3=8!/(8-3)!=8!/5!=336。

##### 知识点 06｜重复字母为什么要除以阶乘｜Arrangements with repeated letters

**题目｜Question.** 排列单词 LEVEL 的字母，有多少种不同排列？

**正确答案｜Correct answer.** 共有5个位置，若字母都不同有5!。L重复2次、E重复2次，交换相同字母不产生新排列，所以数量=5!/(2!2!)=120/4=30。

##### 知识点 07｜排列与组合的分界｜Permutation versus combination

“从8人中选3人”本身没有说明职位，通常是组合；“选主席、秘书、财务员”才是排列。不要看见选人就机械用nCr。重复字母题也不能直接用nPr，因为对象不全不同。

##### 英文概念串联｜Connected explanation in English

A permutation is built from ordered slots. If r positions are filled from n distinct objects without replacement, the numbers of choices are n, n-1, and so on, giving nPr. The factorial formula is only a compact version of this product. Writing the slots explicitly is especially useful when the first position, adjacency or another restriction changes the number of choices.

##### 英文方法说明｜Method in English

Repeated objects require a different correction. Start with the factorial count as if all objects were labelled, then divide by the factorial of each repeated group because exchanging identical objects produces no visible new arrangement. For two objects that must be adjacent, treat them as a block and remember to count their internal orders.

#### 5.2.2 组合与限制条件｜Combinations and restrictions

##### 知识点 01｜只选成员而不安排顺序｜Selections without order

**组合（combination）**解决“只在乎选了谁、不在乎排列次序”的问题。从n个不同对象选r个，数量 nCr=n!/[r!(n-r)!]。分母r!消除同一组选中者的内部排列重复。

**English explanation.** A combination counts selections, not arrangements. The denominator r! removes the r! orders of the same selected group. For restrictions, translate the wording into disjoint cases or use a complement, then state what each term counts.

##### 知识点 02｜nCr 中两个阶乘的含义｜Why the combination formula divides

8C3=8!/(3!5!)。约分：8×7×6×5!/(3×2×1×5!)=(8×7×6)/6=56。答案56表示56个不同委员会，不是56种职位安排。

##### 知识点 03｜从排列推导组合｜Deriving nCr from nPr

先按顺序选3人会得到8P3=336，但每个三人委员会被计算3!=6次，因为三人内部有6种顺序。因此8C3=8P3/3!=336/6=56。这就是组合公式中r!的意义。

##### 知识点 04｜exactly、at least 与 at most｜Translating restrictions

先做“交换测试”：交换两名已选者，结果是否仍是同一组？若是，用nCr。限制题优先翻译为 exactly、at least、at most，再分互斥情况相加；“至少一个”常用总数减一个都没有。

##### 知识点 05｜八人选三名委员｜Choosing an unranked committee

**题目｜Question.** 8个人中选3名委员，没有职位差别。求方法、公式与答案。

**正确答案｜Correct answer.** 顺序不重要，用组合。8C3=8!/[3!(8-3)!]=8!/(3!5!)=(8×7×6)/(3×2×1)=56。规范写法：There are **56 possible committees**。

##### 知识点 06｜至少一个条件的补集法｜Using a complement for at least one

**题目｜Question.** 5男4女中选3人，至少1女，有多少种？

**正确答案｜Correct answer.** 总选法9C3=84。减去全男5C3=10，所以至少1女=84-10=74。也可分1女、2女、3女相加，但补集更短。

##### 知识点 07｜分情况必须互斥｜Making cases disjoint

at least 1不等于exactly 1；at most 2包含0、1、2。分情况相加前必须保证情况互斥。若先选委员会再分配职位，应先组合再排列，并把两个阶段相乘。

##### 英文概念串联｜Connected explanation in English

A combination counts groups, not orders. Ordered selection gives nPr, but each group of r chosen objects appears in r factorial internal orders. Dividing by r factorial gives nCr. Thus eight people choosing three committee members gives 8P3 divided by 3 factorial, which is 336 divided by 6, or 56 committees.

##### 英文方法说明｜Method in English

Translate restrictions before calculating. Exactly two means one case only; at least one means one or more and is often shorter by complement; at most two includes zero, one and two. If a committee is selected and offices are then assigned, the selection and allocation are successive stages, so multiply the combination count by the number of internal arrangements.

### 三、核心词汇表｜Core vocabulary

- **multiplication principle**｜乘法原理：multiply the choices available at successive stages
- **factorial**｜阶乘：n! = n(n-1)...2x1, with 0! = 1
- **permutation**｜排列：a selection or arrangement in which order matters
- **combination**｜组合：a selection in which order does not matter
- **ordered selection**｜有序选择：a choice for which changing positions creates a new result
- **unordered selection**｜无序选择：a group whose internal order creates no new result
- **distinct objects**｜互不相同的对象：objects that remain distinguishable after arrangement
- **repeated objects**｜重复对象：identical objects whose swaps do not create new arrangements
- **arrangement**｜排列方式：a particular ordering of objects
- **selection**｜选取：a choice of members from a larger set
- **restriction**｜限制条件：a condition reducing the permitted outcomes
- **adjacent**｜相邻：next to each other in a line
- **together**｜在一起：treated as one block in a required-adjacency problem
- **not together**｜不相邻：counted efficiently by total minus together
- **block method**｜捆绑法：treat required adjacent objects as one unit
- **complement method**｜补集法：count all outcomes and subtract forbidden outcomes
- **exactly**｜恰好：the stated number and no other number
- **at least**｜至少：the stated number or more
- **at most**｜至多：the stated number or fewer
- **case**｜分类情况：one disjoint possibility in a count
- **mutually exclusive cases**｜互斥分类：cases that cannot describe the same outcome
- **committee**｜委员会：a typical unordered selection unless offices are specified
- **office**｜职位：a distinct role that makes order matter
- **row**｜一排：a linear arrangement with a first and last position
- **overcounting**｜重复计数：counting one outcome more than once

### 四、单元练习｜Unit practice（共 14 题）

#### 2.1 从逐位置选择推出 nPr｜Deriving nPr from ordered slots

Eight runners compete for gold, silver and bronze. Calculate the number of possible podium orders from first principles.

#### 2.2 相邻限制的捆绑法｜Keeping two objects together

Six different books are arranged on a shelf. Two particular books must stay together. Find the number.

#### 2.3 首位不能为零的密码｜A code with a restricted first digit

How many 4-digit codes can be made from 0-9 without repetition if the first digit cannot be 0?

#### 2.4 选择与辨析｜Multiple choice

Eight students fill three different offices. How many allocations are possible?
A 8C3  B 3^8  C 8P3  D 8!/3!

#### 2.5 综合应用 2｜Extended application 2

Show why nPr=n!/(n−r)! rather than n!/r!.

#### 2.6 综合应用 3｜Extended application 3

A student calculates 8C3 for president, secretary and treasurer. Explain the error and give the correct answer.

#### 2.7 综合应用 4｜Extended application 4

Explain in English why LEVEL has 5!/(2!2!) different arrangements.

#### 2.8 恰好两名女生的选择｜Selecting exactly two girls

Choose 4 students from 7 boys and 5 girls, with exactly 2 girls.

#### 2.9 先选委员会再选主席｜Selection followed by allocation

A committee of 4 is chosen from 10 people, then a chair is selected from the committee.

#### 2.10 选择与辨析｜Multiple choice

How many committees of 3 can be selected from 8 people?
A 24  B 56  C 336  D 512

#### 2.11 综合应用 1｜Extended application 1

Eight people are available and three are chosen as an unranked committee. Derive the answer without treating nCr as a calculator key.

#### 2.12 综合应用 2｜Extended application 2

From 6 women and 5 men, choose a committee of 4 containing exactly 2 women. Give every factor a meaning.

#### 2.13 综合应用 3｜Extended application 3

A student answers “at least one girl” with 4C1×5C2. Identify what was counted and complete the correct calculation for 4 girls and 5 boys choosing 3.

#### 2.14 综合应用 4｜Extended application 4

A committee of 3 is chosen from 8 people. Explain in English why the answer is 56 and not 336.

### 五、练习答案与解析｜Answers and explanations（共 14 题）

#### 2.1 从逐位置选择推出 nPr｜Deriving nPr from ordered slots

**完整解答｜Full solution.** Gold can be awarded in 8 ways. After that, silver has 7 remaining choices and bronze has 6. By the multiplication principle, total=8×7×6=336. In compact notation, 8P3=8!/(8−3)!=8!/5!=336.

#### 2.2 相邻限制的捆绑法｜Keeping two objects together

**完整解答｜Full solution.** Treat the pair as one block: there are 5 objects to arrange, giving 5!. The pair can be internally ordered in 2! ways. Total=5!×2=240.

#### 2.3 首位不能为零的密码｜A code with a restricted first digit

**完整解答｜Full solution.** First digit:9 choices (1-9). Then 9,8,7 choices remain. Total=9×9×8×7=4536. A code restriction is handled position by position.

#### 2.4 选择与辨析｜Multiple choice

**完整解答｜Full solution.** C - 8P3=8×7×6=336, because the three offices are distinct.

#### 2.5 综合应用 2｜Extended application 2

**完整解答｜Full solution.** Filling r ordered positions gives n(n−1)…(n−r+1), a product of exactly r descending factors. Since n!=n(n−1)…(n−r+1)(n−r)!, dividing n! by (n−r)! removes the unused tail and leaves those r factors.

#### 2.6 综合应用 3｜Extended application 3

**完整解答｜Full solution.** The three offices are different: changing who is president creates a different allocation. Order therefore matters. Use 8P3=8×7×6=336, not 8C3=56. The combination answer would merge the 3!=6 office orders belonging to each selected trio.

#### 2.7 综合应用 4｜Extended application 4

**完整解答｜Full solution.** If all five letters were distinct, there would be 5! arrangements. The two Ls can be exchanged in 2! ways without creating a new word, and the two Es can also be exchanged in 2! invisible ways. Therefore the number of distinct arrangements is 5!/(2!2!)=30.

#### 2.8 恰好两名女生的选择｜Selecting exactly two girls

**完整解答｜Full solution.** Choose girls and boys independently: 5C2×7C2=10×21=210. “Exactly 2 girls” forces exactly 2 boys.

#### 2.9 先选委员会再选主席｜Selection followed by allocation

**完整解答｜Full solution.** Choose committee:10C4. Choose chair from its 4 members:4 choices. Total=10C4×4=840.

#### 2.10 选择与辨析｜Multiple choice

**完整解答｜Full solution.** B - 56. Order does not matter, so 8C3=8!/(3!5!)=56.

#### 2.11 综合应用 1｜Extended application 1

**完整解答｜Full solution.** Ordered selection first gives 8P3=8×7×6=336. For any chosen trio, the same three people appear in 3!=6 internal orders, but an unranked committee counts all six as one result. Hence 8C3=8P3/3!=336/6=56. Equivalently, 8C3=8!/[3!(8−3)!]=8!/(3!5!)=56.

#### 2.12 综合应用 2｜Extended application 2

**完整解答｜Full solution.** Choose 2 of the 6 women: 6C2=15. Independently choose 2 of the 5 men: 5C2=10. Each women-choice can be paired with each men-choice, so multiply: 6C2×5C2=15×10=150 committees.

#### 2.13 综合应用 3｜Extended application 3

**完整解答｜Full solution.** The expression 4C1×5C2 counts **exactly one girl**, not at least one. Use the complement: all committees=9C3=84; committees with no girl=5C3=10. Therefore at least one girl=84−10=74.

#### 2.14 综合应用 4｜Extended application 4

**完整解答｜Full solution.** A committee has no different positions, so changing the order in which the same three people are selected does not create a new committee. The ordered count 8P3=336 counts each trio 3!=6 times. Dividing by 6 gives 8C3=56 distinct committees.

### 六、自学检查清单｜Self-study checklist

- [ ] I can decide whether order matters by applying the exchange test.
- [ ] I can derive nPr from the multiplication principle rather than treating it as a calculator command.
- [ ] I can derive nCr by removing the r! internal orders of each selected group.
- [ ] I can count arrangements with repeated objects by dividing by repetition factorials.
- [ ] I can solve together/not-together restrictions by block or complement methods.
- [ ] I can translate exactly, at least and at most into complete disjoint cases.
- [ ] I can combine selection and allocation stages and explain every factor.
- [ ] I know that circular arrangements are outside the S1 syllabus.

## 单元 3｜5.3 概率｜Probability

### 一、单元导读｜Unit introduction

本单元把文字情境转化为事件、样本空间、树图和概率运算。先区分 union、intersection、complement，再区分 mutually exclusive 与 independent；最后学习条件概率。计算之前必须知道样本空间是否等可能、抽取是否放回，以及第二步概率会不会因第一步结果改变。

**与国内课程衔接｜Connection with Chinese curriculum.** 国内初中概率多使用列举和树状图，S1 在此基础上加入事件符号、独立性检验和 P(A|B)。Cambridge 题目经常把组合计数与概率结合，并要求用精确分数或合理精度说明结果。

**学习路线｜Learning route.** 等可能结果与列举 → 加法/乘法 → 互斥与独立 → 补集 → 不放回树图 → conditional probability → 反向条件问题。

### 二、知识点精讲｜Detailed teaching

#### 5.3.1 概率加法与乘法法则｜Probability rules

##### 知识点 01｜并集、交集与补集｜Union, intersection and complement

事件A∪B表示A或B至少一个发生；A∩B表示同时发生。互斥事件不能同时发生；独立事件互不改变概率。两组词不能混用。

**English explanation.** Addition handles an inclusive “or”; multiplication handles a sequence or intersection. Mutually exclusive events have zero intersection. Independent events may occur together, but one event does not change the probability of the other.

##### 知识点 02｜互斥与独立使用不同公式｜Exclusive versus independent events

P(A∪B)=P(A)+P(B)-P(A∩B)。若互斥，交集为0。独立时P(A∩B)=P(A)P(B)。补集P(A′)=1-P(A)。

##### 知识点 03｜加法公式为何减去交集｜Avoiding double counting

加法公式减去交集，是因为P(A)+P(B)把同时发生部分算了两次。独立乘法来自P(A|B)=P(A)：P(A∩B)=P(A|B)P(B)=P(A)P(B)。

##### 知识点 04｜把文字准确翻译成事件｜Translating probability language

先把文字改写成符号：either/or→union，both/and→intersection，not→complement。再判断是否给出mutually exclusive或independent。最后代公式，并检查概率在0到1之间。

##### 知识点 05｜包含交集的并集计算｜Calculating an inclusive union

**题目｜Question.** P(A)=0.55，P(B)=0.40，P(A∩B)=0.18，求P(A∪B)。

**正确答案｜Correct answer.** 0.55+0.40-0.18=0.77。必须减交集，否则得到0.95并重复计算同时发生部分。

##### 知识点 06｜恰好一个事件发生｜Exactly one of two events

**题目｜Question.** A、B独立，P(A)=0.3，P(B)=0.6，求恰好一个发生。

**正确答案｜Correct answer.** P(A∩B′)+P(A′∩B)=0.3×0.4+0.7×0.6=0.12+0.42=0.54。两条路径互斥，所以相加。

##### 知识点 07｜非零互斥事件不独立｜Why exclusive events are dependent

互斥且概率都非零的事件不可能独立：若互斥，P(A∩B)=0；若独立，应为P(A)P(B)>0。题目中的“or”通常是inclusive or，除非明确说only one。

##### 英文概念串联｜Connected explanation in English

Probability language determines the operation. Or describes a union and normally includes the overlap; and describes an intersection; not describes a complement. Addition combines alternative, disjoint routes, while multiplication follows successive stages along one route. If two events overlap, subtract the intersection once after adding their probabilities.

##### 英文方法说明｜Method in English

Mutually exclusive and independent describe different relationships. Exclusive events cannot occur together. Independent events can occur together, but knowledge of one does not change the probability of the other. To test independence, compare the calculated intersection with the product of the two marginal probabilities; a verbal claim alone is not enough.

#### 5.3.2 条件概率与树图｜Conditional probability and tree diagrams

##### 知识点 01｜条件改变样本空间｜A condition changes the sample space

条件概率P(A|B)表示已知B发生后A发生的概率。样本空间被缩小到B，所以分母是P(B)：P(A|B)=P(A∩B)/P(B)。

**English explanation.** A tree diagram makes conditional structure visible. Multiply along a path, add disjoint paths, and use the total probability of the given event as the denominator when reversing a condition.

##### 知识点 02｜树图的分支、路径与总概率｜Branches, paths and total probability

树图每一组分支概率和为1。沿同一路径相乘得到联合概率；满足同一目标的互斥路径相加。不放回抽样会改变第二层分子与分母。

##### 知识点 03｜条件概率公式的来源｜Deriving the conditional formula

P(A∩B)既可写P(A|B)P(B)，也可写P(B|A)P(A)。这不是假设独立，而是条件概率定义的重排。只有独立时P(A|B)=P(A)。

##### 知识点 04｜不放回时逐层更新概率｜Updating without replacement

第一层写第一次事件；第二层从每个结果分别出发。每条枝先写条件概率，再沿路径乘。题目问given that时，最后用目标交集除以given事件总概率。

##### 知识点 05｜两次抽取同色｜Adding two disjoint paths

**题目｜Question.** 袋中4红3蓝，不放回抽2球，求两球同色。

**正确答案｜Correct answer.** 红红=4/7×3/6=2/7；蓝蓝=3/7×2/6=1/7；同色=3/7。两条路径互斥，所以相加。

##### 知识点 06｜从检测结果反推患病概率｜Reversing a medical-test condition

**题目｜Question.** 某病患病率0.02；检测对患病者阳性0.95，对未患病者假阳性0.04。求阳性概率。

**正确答案｜Correct answer.** P(+)=0.02×0.95+0.98×0.04=0.019+0.0392=0.0582。若问P(disease|+)，再算0.019/0.0582≈0.326。

##### 知识点 07｜P(A|B) 与 P(B|A) 不可互换｜The direction of conditioning

P(A|B)通常不等于P(B|A)。medical test题中“阳性者患病率”不能直接写检测灵敏度；还必须考虑未患病人口规模和假阳性。

##### 英文概念串联｜Connected explanation in English

Conditional probability changes the reference population. P(A given B) asks what fraction of the B outcomes also satisfy A, which explains why the denominator is P(B). The direction matters: P(positive given disease) is not the same question as P(disease given positive). A tree diagram helps keep the two directions and their denominators separate.

##### 英文方法说明｜Method in English

At every split of a tree, branch probabilities sum to one. Multiply along a complete path because all events on that path must occur; add different paths only when they are alternative ways to meet the target. Without replacement, update both numerator and denominator after the first draw. For a reverse conditional probability, divide the required joint path by the total probability of the stated condition.

### 三、核心词汇表｜Core vocabulary

- **sample space**｜样本空间：the set of all possible elementary outcomes
- **elementary event**｜基本事件：one indivisible outcome in the sample space
- **equally likely**｜等可能：having the same probability
- **event**｜事件：a set of outcomes of interest
- **union**｜并集：A or B or both, written A union B
- **intersection**｜交集：A and B together, written A intersection B
- **complement**｜补集：the event that A does not occur
- **inclusive or**｜包含式或：A or B including the possibility that both occur
- **mutually exclusive**｜互斥：events that cannot occur together
- **independent**｜独立：events for which one does not change the probability of the other
- **dependent**｜不独立：events for which knowledge of one changes another probability
- **conditional probability**｜条件概率：a probability calculated within a reduced sample space
- **given that**｜已知：words indicating the condition after the vertical bar
- **tree diagram**｜树图：a branching representation of sequential probabilities
- **branch**｜树枝：one possible outcome at a stage of a tree
- **path**｜路径：a sequence of branches describing a joint outcome
- **with replacement**｜放回抽取：returning the item so later probabilities are unchanged
- **without replacement**｜不放回抽取：removing the item so later probabilities change
- **joint probability**｜联合概率：the probability that specified events occur together
- **addition rule**｜加法规则：a rule for combining alternative events
- **multiplication rule**｜乘法规则：a rule for probabilities along a path
- **enumeration**｜列举：systematically listing possible outcomes
- **fair**｜公平的：giving equally likely outcomes in the stated model
- **false positive**｜假阳性：a positive test result when the condition is absent
- **sensitivity**｜灵敏度：the probability of a positive result given the condition

### 四、单元练习｜Unit practice（共 14 题）

#### 3.1 含交集的并集概率｜Union with an intersection

Given P(A)=0.62, P(B)=0.47 and P(A∩B)=0.21, find P(A∪B) and explain the subtraction.

#### 3.2 检验事件是否独立｜Testing independence

P(A)=0.7, P(B)=0.5 and P(A∪B)=0.9. Find P(A∩B) and decide whether independent.

#### 3.3 证明互斥不等于独立｜Proving exclusive is not independent

A student says non-zero mutually exclusive events are independent. Prove that this is false.

#### 3.4 选择与辨析｜Multiple choice

A and B are independent with probabilities 0.4 and 0.5. Find P(A∩B).
A 0  B 0.2  C 0.9  D 1

#### 3.5 迁移应用｜Transfer problem

Find P(neither A nor B) when P(A∪B)=0.77.

#### 3.6 综合应用 2｜Extended application 2

A and B are independent with P(A)=0.4 and P(B)=0.7. Find the probability that exactly one occurs.

#### 3.7 综合应用 4｜Extended application 4

Explain in English the difference between “mutually exclusive” and “independent”.

#### 3.8 不放回抽样的条件概率｜Conditional probability without replacement

A bag contains 5 red and 3 blue balls. Two are drawn without replacement. Find P(second is red | first is blue).

#### 3.9 为什么不能倒置条件｜Why the condition cannot be reversed

A test has sensitivity 0.9. A student concludes P(disease | positive)=0.9. Explain why this is wrong.

#### 3.10 阳性之后真正患病的概率｜Probability of disease after a positive test

A disease prevalence is 0.01, sensitivity 0.95 and false-positive rate 0.03. Find and interpret P(disease | positive).

#### 3.11 选择与辨析｜Multiple choice

A bag has 3 white and 2 black balls. Two are drawn without replacement. Find P(white then black).
A 1/5  B 3/10  C 2/5  D 1/2

#### 3.12 结构化计算｜Structured calculation

Given P(A∩B)=0.24 and P(B)=0.4, find P(A|B).

#### 3.13 迁移应用｜Transfer problem

When can a without-replacement model be approximated as independent?

#### 3.14 综合应用 2｜Extended application 2

Use the definition of conditional probability when P(A∩B)=0.18 and P(B)=0.30.

### 五、练习答案与解析｜Answers and explanations（共 14 题）

#### 3.1 含交集的并集概率｜Union with an intersection

**完整解答｜Full solution.** P(A∪B)=P(A)+P(B)−P(A∩B)=0.62+0.47−0.21=0.88. The intersection is subtracted once because it was included once in P(A) and once again in P(B).

#### 3.2 检验事件是否独立｜Testing independence

**完整解答｜Full solution.** Intersection=0.7+0.5-0.9=0.3. Since P(A)P(B)=0.35≠0.3, the events are not independent.

#### 3.3 证明互斥不等于独立｜Proving exclusive is not independent

**完整解答｜Full solution.** Mutually exclusive gives P(A∩B)=0. Independence would require P(A∩B)=P(A)P(B). If both probabilities are non-zero, P(A)P(B)>0, contradicting the zero intersection. Therefore non-zero mutually exclusive events are dependent.

#### 3.4 选择与辨析｜Multiple choice

**完整解答｜Full solution.** B - 0.2, because independence gives 0.4×0.5.

#### 3.5 迁移应用｜Transfer problem

**完整解答｜Full solution.** Neither is the complement of the union:1-0.77=0.23.

#### 3.6 综合应用 2｜Extended application 2

**完整解答｜Full solution.** Exactly one means (A∩B′) or (A′∩B). Independence gives 0.4×0.3 + 0.6×0.7 = 0.12+0.42=0.54. The two cases cannot occur together, so their probabilities are added.

#### 3.7 综合应用 4｜Extended application 4

**完整解答｜Full solution.** Mutually exclusive events cannot occur together, so their intersection has probability zero. Independent events may occur together, but knowing that one occurred does not change the probability of the other; equivalently P(A∩B)=P(A)P(B).

#### 3.8 不放回抽样的条件概率｜Conditional probability without replacement

**完整解答｜Full solution.** Once a blue ball has been removed, 7 balls remain: 5 red and 2 blue. Therefore P(second red | first blue)=5/7. The condition changes the sample space before the second probability is written.

#### 3.9 为什么不能倒置条件｜Why the condition cannot be reversed

**完整解答｜Full solution.** Sensitivity is P(positive | disease), not P(disease | positive). Reversing the condition changes the denominator. To find P(disease | positive), calculate the disease-and-positive path and divide by total positive probability, including false positives.

#### 3.10 阳性之后真正患病的概率｜Probability of disease after a positive test

**完整解答｜Full solution.** P(D∩+)=0.01×0.95=0.0095. P(+)=0.0095+0.99×0.03=0.0392. Hence P(D|+)=0.0095/0.0392≈0.242. **Interpretation:** about 24.2% of people who test positive actually have the disease under this model.

#### 3.11 选择与辨析｜Multiple choice

**完整解答｜Full solution.** B - 3/5×2/4=3/10.

#### 3.12 结构化计算｜Structured calculation

**完整解答｜Full solution.** P(A|B)=0.24/0.4=0.6. The denominator is the probability of the given event B.

#### 3.13 迁移应用｜Transfer problem

**完整解答｜Full solution.** When the population is very large relative to the sample, removal changes probabilities negligibly; state this as an approximation, not exact equality.

#### 3.14 综合应用 2｜Extended application 2

**完整解答｜Full solution.** P(A|B)=P(A∩B)/P(B)=0.18/0.30=0.60. Dividing by P(B) rescales the part of B that also lies in A relative to the whole reduced sample space B.

### 六、自学检查清单｜Self-study checklist

- [ ] I can build an equiprobable sample space and count favourable outcomes.
- [ ] I can translate or, and, not and given that into event notation.
- [ ] I can avoid double-counting an intersection when adding probabilities.
- [ ] I can distinguish mutually exclusive events from independent events.
- [ ] I can test independence by comparing P(A and B) with P(A)P(B).
- [ ] I can construct a tree whose branches at every split sum to 1.
- [ ] I can update probabilities correctly for sampling without replacement.
- [ ] I can multiply along a path and add alternative disjoint paths.
- [ ] I can calculate P(A given B) with the correct denominator and interpret it in context.

## 单元 4｜5.4 离散随机变量｜Discrete random variables

### 一、单元导读｜Unit introduction

本单元把随机结果编码为离散随机变量 X。先建立概率分布表并计算 E(X) 与 Var(X)，再学习两种标准模型：二项分布统计固定次数中的成功数，几何分布统计第一次成功出现在哪一次。能否使用模型比套公式更重要。

**与国内课程衔接｜Connection with Chinese curriculum.** 国内教材中的随机变量、期望与方差在这里被放进实际模型。Cambridge 要求使用 B(n,p) 和 Geo(p) 记号，准确翻译 exactly、at least、at most、on the rth trial、after r trials，并识别独立性和恒定成功概率。

**学习路线｜Learning route.** 定义 X 与列分布表 → 概率和为 1 → E(X)、E(X²)、Var(X) → 净收益 → binomial 四条件 → 单点/累积概率 → geometric 等待时间。

### 二、知识点精讲｜Detailed teaching

#### 5.4.1 离散随机变量与期望方差｜Discrete random variables

##### 知识点 01｜从随机结果定义 X｜Defining a discrete random variable

离散随机变量X把随机结果映射为可数数值。概率分布表必须满足每个p≥0且Σp=1。E(X)是长期平均，不要求是X可取的数。

**English explanation.** A probability distribution is a complete model of a discrete random variable. Expectation describes its long-run average; variance describes spread around that average. A linear change affects location and spread differently.

##### 知识点 02｜概率表、期望与方差公式｜Distribution, expectation and variance

E(X)=Σxp；E(X²)=Σx²p；Var(X)=E(X²)-[E(X)]²。概率表还必须满足每个 p≥0 且 Σp=1。

##### 知识点 03｜从定义推出方差快捷公式｜Deriving the variance identity

令 μ=E(X)。从定义 Var(X)=E[(X-μ)²] 展开：E(X²-2μX+μ²)=E(X²)-2μE(X)+μ²=E(X²)-μ²，因此得到快捷公式。

##### 知识点 04｜先补概率再计算矩｜A reliable distribution-table method

先用Σp=1求未知常数；再增列xp与x²p；分别求和。若X表示净收益，先从奖金中扣成本，再计算期望，不能把gross prize当profit。

##### 知识点 05｜含未知常数的概率表｜Finding a missing probability

**题目｜Question.** X取0,1,2，概率k,2k,3k。求k与E(X)。

**正确答案｜Correct answer.** 6k=1，所以k=1/6。E(X)=0+1×2/6+2×3/6=4/3。

##### 知识点 06｜从 E(X²) 得到 Var(X)｜Calculating variance from the second moment

**题目｜Question.** 上一分布求variance。

**正确答案｜Correct answer.** E(X²)=0+1×2/6+4×3/6=7/3。Var=7/3-(4/3)²=5/9。

##### 知识点 07｜净收益而不是奖金｜Net gain rather than gross prize

E(X²)不等于[E(X)]²。方差出现负数说明算术错误。期望收益为正不保证每次盈利，只说明大量重复后的平均净结果。

##### 英文概念串联｜Connected explanation in English

A discrete random variable replaces verbal outcomes by numerical values. Its probability table is complete only when every probability is non-negative and the total is one. Expectation is a probability-weighted long-run average; it need not be one of the values that X can actually take. Variance measures squared spread about that expected value.

##### 英文方法说明｜Method in English

Use separate columns for xp and x squared p. Find E(X) and E(X squared), then subtract the square of E(X). In a game, define X as net gain if the question asks about profit: subtract the entry cost from every prize outcome before taking the expectation. A negative expected value describes a long-run average loss, not the result of every individual play. Linear combinations of random variables are studied in Paper 6, not in this S1 unit.

#### 5.4.2 二项分布：建模、概率与累积事件｜Binomial distribution

##### 知识点 01｜二项模型的四个条件｜Four binomial conditions

X~B(n,p)表示n次Bernoulli试验中的成功次数。必须满足：固定n、每次只有success/failure、试验独立、成功概率p恒定。

**English explanation.** A binomial variable counts successes. The combination chooses the positions of the successes; the powers give the probability of each success-failure pattern. Always state the random variable and verify the four assumptions.

##### 知识点 02｜单点概率、均值与方差｜Probability, mean and variance

P(X=r)=nCr p^r(1-p)^(n-r)。E(X)=np，Var(X)=np(1-p)。符号翻译：at least r是X≥r；more than r是X>r；at most r是X≤r。

##### 知识点 03｜组合数为何出现在公式中｜Why nCr appears

某一条恰有r次成功的序列概率是p^r(1-p)^(n-r)。成功可以出现在n个位置中的任意r个，共nCr种，因此乘上组合数。

##### 知识点 04｜把至少、至多翻译成事件｜Translating cumulative events

第一行定义X并写分布。第二行把文字翻译成事件。第三行决定单项、累积或补集。第四行代公式/计算器。最后写概率并保留3 significant figures左右。

##### 知识点 05｜恰好三次成功｜Exactly three successes

**题目｜Question.** 硬币正面概率0.4，抛8次，恰3次正面。

**正确答案｜Correct answer.** 令X为正面次数，X~B(8,0.4)。P(X=3)=8C3(0.4)^3(0.6)^5≈0.2787，答案0.279。

##### 知识点 06｜至少一次的补集法｜Complement for at least one

**题目｜Question.** 同一模型，至少1次正面。

**正确答案｜Correct answer.** P(X≥1)=1-P(X=0)=1-(0.6)^8≈0.9832。用补集只需一项。

##### 知识点 07｜不放回通常破坏二项条件｜Why sampling without replacement is different

“不放回抽样”通常使p改变，不是严格二项。at least 3不能输入P(X=3)。计算器binomcdf常给P(X≤r)，求P(X≥r)需1-P(X≤r-1)。

##### 英文概念串联｜Connected explanation in English

A binomial variable counts successes in a fixed number of independent trials, with two outcomes per trial and a constant success probability. The word success only names the counted outcome; it need not be desirable. If sampling without replacement changes the success probability appreciably, the exact model is not binomial.

##### 英文方法说明｜Method in English

In P(X=r), nCr selects the r success positions, p to the power r gives the success factors, and (1-p) to the power n-r gives the failure factors. Translate the event before using a table or calculator. At least r means one minus P(X at most r-1), not one minus P(X at most r). State X and its B(n,p) distribution before the calculation.

#### 5.4.3 几何分布与等待时间｜Geometric distribution

##### 知识点 01｜第一次成功的等待模型｜Waiting for the first success

几何分布描述独立重复试验中第一次成功出现的试验编号。若每次成功概率p不变，X的可能值为1,2,3,...。

**English explanation.** A geometric variable is a waiting-time model. Count the failures before the first success carefully. “On trial r” includes a final factor p, while “after trial r” means r failures and does not.

##### 知识点 02｜on、after 与 within 的公式｜Formulae for three common wordings

P(X=r)=(1-p)^(r-1)p；P(X>r)=(1-p)^r；P(X≤r)=1-(1-p)^r。E(X)=1/p。

##### 知识点 03｜r-1 次失败后再成功｜Deriving the geometric probability

第一次成功在第r次意味着前r-1次全部失败，随后成功，所以概率是(1-p)^(r-1)p。超过r次仍未成功意味着前r次全失败。

##### 知识点 04｜先数失败次数｜Counting failures before success

先分清“on trial r”“after trial r”“within r trials”。写出失败次数，再写最后是否需要乘p。检查X从1开始，不存在第0次首次成功。

##### 知识点 05｜首次成功在第4次｜First success on trial four

**题目｜Question.** 每次成功率0.25，首次成功在第4次。

**正确答案｜Correct answer.** 前三次失败、第四次成功：P(X=4)=0.75^3×0.25≈0.1055。

##### 知识点 06｜成功概率必须保持不变｜The constant-probability condition

P(X=4)不是0.75^4，也不是0.25^4。前者表示前4次全失败，后者表示4次全成功。题目若成功概率随次数改变，就不能使用几何模型。

##### 英文概念串联｜Connected explanation in English

A geometric variable records the trial number of the first success, so its possible values begin at one. First success on trial r means r-1 failures followed by one success. First success after trial r means that all first r trials fail, whereas within r trials means at least one success occurs among those r trials.

##### 英文方法说明｜Method in English

Write the failure sequence before writing the formula. This makes the exponents visible and prevents the common extra-failure error. The model requires independent trials and the same success probability each time. Its expectation 1/p is a long-run average waiting time and need not be an integer or a guaranteed waiting time.

### 三、核心词汇表｜Core vocabulary

- **random variable**｜随机变量：a numerical value assigned to each random outcome
- **discrete random variable**｜离散随机变量：a random variable with countable possible values
- **probability distribution**｜概率分布：all possible values of X with their probabilities
- **expected value**｜期望：the probability-weighted long-run average
- **second moment**｜二阶矩：E(X squared), used in the variance formula
- **variance**｜方差：E(X squared) minus the square of E(X)
- **net gain**｜净收益：prize or revenue after subtracting the cost
- **long-run average**｜长期平均：the average approached over many repetitions
- **Bernoulli trial**｜伯努利试验：one trial with success or failure
- **success**｜成功：the outcome being counted, not necessarily something desirable
- **failure**｜失败：the alternative outcome to success
- **binomial distribution**｜二项分布：the count of successes in a fixed number of independent trials
- **fixed number of trials**｜固定试验次数：a required condition for a binomial model
- **constant probability**｜恒定概率：the same success probability on every trial
- **cumulative probability**｜累积概率：the probability up to or beyond a stated count
- **binomial coefficient**｜二项系数：nCr, choosing the positions of the successes
- **geometric distribution**｜几何分布：the trial number of the first success
- **waiting time**｜等待时间：the number of trials needed to reach the first success
- **on trial r**｜第 r 次恰好成功：r-1 failures followed by a success
- **after trial r**｜超过 r 次才成功：failure throughout the first r trials
- **within r trials**｜r 次以内成功：at least one success among the first r trials
- **independent trials**｜独立试验：trials whose outcomes do not affect later probabilities
- **parameter**｜参数：a number such as n or p defining a distribution
- **model**｜模型：a mathematical description with stated assumptions
- **gross prize**｜总奖金：the payment before entry cost is deducted
- **probability table**｜概率表：a table pairing each value x with P(X=x)
- **at least one**｜至少一次：usually calculated efficiently as one minus no successes
- **standard deviation**｜标准差：the square root of a random variable's variance

### 四、单元练习｜Unit practice（共 18 题）

#### 4.1 补全分布并计算期望方差｜Completing a distribution

X takes 0, 1, 3 with probabilities k, 2k, 2k. Find k, E(X) and Var(X).

#### 4.2 将奖金改写为净收益｜Modelling net gain

A game costs $4 and pays $12 with probability 0.25, otherwise $0. A student uses outcomes 12 and 0. Repair the model.

#### 4.3 解释负期望的现实含义｜Interpreting a negative expectation

Explain an expected net gain of −$1 in English.

#### 4.4 迁移应用｜Transfer problem

A game costs $3 and pays $10 with probability 0.2, otherwise $0. Find expected net gain.

#### 4.5 解释二项概率中的每个因子｜Explaining every binomial factor

A biased coin has P(head)=0.3 and is tossed 6 times. Find P(exactly 2 heads) by explaining every factor.

#### 4.6 订正 at least 的计算器输入｜Correcting an at-least event

A student enters binomcdf(n,p,3) for “at least 3 successes”. Correct the event and input logic.

#### 4.7 判断不放回抽样能否建模｜Checking the binomial conditions

State whether sampling 10 items without replacement from a batch of 20 gives a binomial model.

#### 4.8 选择与辨析｜Multiple choice

X~B(10,0.2). Which expression gives P(X≥1)?
A 0.2^10  B 1-0.2^10  C 1-0.8^10  D 10×0.2

#### 4.9 结构化计算｜Structured calculation

A machine makes a defective item with probability 0.03 independently. Find probability exactly 2 of 20 are defective.

#### 4.10 迁移应用｜Transfer problem

Find the mean and standard deviation for B(80,0.35).

#### 4.11 综合应用 2｜Extended application 2

Explain why E(X)=np is plausible for a binomial count.

#### 4.12 首次成功在第5次｜First success on trial five

Success probability is 0.2. Find the probability that the first success occurs on trial 5.

#### 4.13 订正失败次数｜Correcting the number of failures

A student writes P(X=4)=0.7⁴ when p=0.3. Explain exactly which event 0.7⁴ represents and repair the answer.

#### 4.14 区分 on 与 after｜Distinguishing on from after

Explain the difference between “on the sixth trial” and “after the sixth trial”.

#### 4.15 选择与辨析｜Multiple choice

With p=0.3, find the probability that the first success is after trial 4.
A 0.3^4  B 0.7^3×0.3  C 0.7^4  D 1-0.7^4

#### 4.16 结构化计算｜Structured calculation

Find P(X=6) when p=0.2.

#### 4.17 迁移应用｜Transfer problem

Explain the memoryless property.

#### 4.18 综合应用 2｜Extended application 2

Derive P(X≤r)=1−(1−p)^r.

### 五、练习答案与解析｜Answers and explanations（共 18 题）

#### 4.1 补全分布并计算期望方差｜Completing a distribution

**完整解答｜Full solution.** Total probability gives k+2k+2k=5k=1, so k=0.2. E(X)=0(0.2)+1(0.4)+3(0.4)=1.6. E(X²)=0+1(0.4)+9(0.4)=4.0. Hence Var(X)=4.0−1.6²=1.44.

#### 4.2 将奖金改写为净收益｜Modelling net gain

**完整解答｜Full solution.** The random variable must be **net gain**, so the outcomes are 12−4=$8 and 0−4=−$4. Expected net gain=0.25(8)+0.75(−4)=2−3=−$1. Using gross prizes would ignore the certain entry cost.

#### 4.3 解释负期望的现实含义｜Interpreting a negative expectation

**完整解答｜Full solution.** The result does not mean that the player loses exactly $1 in every game. It means that over a very large number of plays under the same probabilities, the average net gain per game is expected to approach −$1.

#### 4.4 迁移应用｜Transfer problem

**完整解答｜Full solution.** Net outcomes are 7 and -3. E=0.2×7+0.8×(-3)=-1. The player loses $1 per game on average.

#### 4.5 解释二项概率中的每个因子｜Explaining every binomial factor

**完整解答｜Full solution.** Choose the 2 head positions in 6C2 ways. Any fixed pattern with 2 heads and 4 tails has probability 0.3²×0.7⁴. Hence P(X=2)=6C2(0.3)²(0.7)⁴=15×0.09×0.2401≈0.324.

#### 4.6 订正 at least 的计算器输入｜Correcting an at-least event

**完整解答｜Full solution.** binomcdf(n,p,3) gives P(X≤3), which is the wrong tail. “At least 3” means X≥3. Use the complement P(X≥3)=1−P(X≤2), so enter 1−binomcdf(n,p,2).

#### 4.7 判断不放回抽样能否建模｜Checking the binomial conditions

**完整解答｜Full solution.** It is not an exact binomial model because removing an item changes the composition of the batch and therefore changes the success probability on later selections. The trials are also not independent.

#### 4.8 选择与辨析｜Multiple choice

**完整解答｜Full solution.** C - 1-P(X=0)=1-(0.8)^10.

#### 4.9 结构化计算｜Structured calculation

**完整解答｜Full solution.** X~B(20,0.03). P(X=2)=20C2(0.03)^2(0.97)^18≈0.0988.

#### 4.10 迁移应用｜Transfer problem

**完整解答｜Full solution.** Mean=np=28. Variance=80×0.35×0.65=18.2, so sd=√18.2≈4.27.

#### 4.11 综合应用 2｜Extended application 2

**完整解答｜Full solution.** Write X as the sum of n success indicators, each equal to 1 for success and 0 for failure. Each indicator has expectation p. Expectations add, even before calculating individual probabilities, so E(X)=p+p+…+p=np.

#### 4.12 首次成功在第5次｜First success on trial five

**完整解答｜Full solution.** Trials 1–4 must fail and trial 5 must succeed. Thus P(X=5)=0.8⁴×0.2=0.08192. There are four failure factors, not five, because the fifth trial is the success.

#### 4.13 订正失败次数｜Correcting the number of failures

**完整解答｜Full solution.** 0.7⁴ means the first four trials all fail, so it represents P(X>4). For the first success **on** trial 4, only the first three trials fail and the fourth succeeds: P(X=4)=0.7³×0.3=0.1029.

#### 4.14 区分 on 与 after｜Distinguishing on from after

**完整解答｜Full solution.** “On the sixth trial” requires five failures followed by a success, so its probability is (1−p)⁵p. “After the sixth trial” means no success in the first six trials, so its probability is (1−p)⁶.

#### 4.15 选择与辨析｜Multiple choice

**完整解答｜Full solution.** C - 0.7^4, because the first four trials must all fail.

#### 4.16 结构化计算｜Structured calculation

**完整解答｜Full solution.** P(X=6)=0.8^5×0.2=0.065536≈0.0655.

#### 4.17 迁移应用｜Transfer problem

**完整解答｜Full solution.** After any number of failures, the probability of success on the next trial is still p because trials are independent; the past does not alter the future model.

#### 4.18 综合应用 2｜Extended application 2

**完整解答｜Full solution.** The complement of “the first success occurs within r trials” is “all of the first r trials fail”. Independence gives failure probability (1−p)^r. Therefore P(X≤r)=1−P(X>r)=1−(1−p)^r.

### 六、自学检查清单｜Self-study checklist

- [ ] I can define X clearly and construct a complete probability distribution table.
- [ ] I can use total probability 1 to find an unknown constant.
- [ ] I can calculate E(X), E(X squared) and Var(X) with separate working columns.
- [ ] I can model net gain by subtracting a certain cost from every outcome.
- [ ] I can check the four conditions before using a binomial distribution.
- [ ] I can explain the combination factor in the binomial probability formula.
- [ ] I can translate exactly, at least, more than and at most into events and complements.
- [ ] I can recognise a geometric waiting-time model and count r-1 failures before the first success.
- [ ] I can distinguish on trial r, after trial r and within r trials.
- [ ] I can state and use binomial mean/variance and geometric mean.

## 单元 5｜5.5 正态分布｜The normal distribution

### 一、单元导读｜Unit introduction

本单元用正态曲线描述连续变量，并把一般正态变量标准化为 Z。需要会由界值求面积、由面积反求界值，也要会用带 continuity correction 的正态分布近似二项分布。草图、参数口径和不等号翻译决定计算方向。

**与国内课程衔接｜Connection with Chinese curriculum.** 国内高中通常先介绍钟形曲线和标准正态分布；S1 更强调完整标准化过程、反求参数，以及离散二项分布到连续正态分布之间的半单位修正。官方要求标准化计算写出完整 working。

**学习路线｜Learning route.** N(mean, variance) → 曲线面积与对称性 → Z=(X-mean)/sd → 单尾/双尾 → inverse normal → 近似条件 np>5、nq>5 → continuity correction。

### 二、知识点精讲｜Detailed teaching

#### 5.5.1 正态分布：标准化与反求界值｜Normal distribution

##### 知识点 01｜均值、方差与曲线面积｜Mean, variance and area

X~N(μ,σ²)是连续、对称、钟形分布。μ决定中心，σ决定伸展程度；第二参数σ²是variance。曲线总面积1，单点概率为0。

**English explanation.** A normal probability is an area. A sketch identifies the correct tail; standardisation measures distance from the mean in standard deviations. In inverse problems, use the area to determine the sign of z before converting back.

##### 知识点 02｜标准化与反标准化｜Standardising and converting back

标准化Z=(X-μ)/σ，把任意正态变量转换为N(0,1)。P(X<a)=P[Z<(a-μ)/σ]。反求a时先从概率得到z，再用a=μ+zσ。

##### 知识点 03｜为什么除以标准差｜Why standardisation divides by sigma

减μ把中心移到0；除σ把一个标准差重新缩放为1。标准化不改变某点处于均值左侧还是右侧，因此z的正负必须与草图一致。

##### 知识点 04｜先画阴影再判断尾部｜Sketching before calculation

画钟形草图，标μ、界值与阴影；写分布；标准化；读表/计算器；利用对称或补集；最后检查概率大小。反求界值时先判断z应正还是负。

##### 知识点 05｜已知界值求概率｜Finding an area from a boundary

**题目｜Question.** X~N(50,3²)，求P(X<56)。

**正确答案｜Correct answer.** z=(56-50)/3=2。P(X<56)=P(Z<2)=0.9772。56在均值右侧2个sd，左侧概率应大于0.5，检查通过。

##### 知识点 06｜已知概率反求界值｜Finding a boundary from an area

**题目｜Question.** 同一分布，求a使P(X<a)=0.10。

**正确答案｜Correct answer.** 下尾10%对应z≈-1.2816。a=50+(-1.2816)×3≈46.2。下尾界值应小于均值，检查通过。

##### 知识点 07｜第二参数是方差｜The second parameter is variance

N(50,9)表示variance=9、sd=3，不是sd=9。upper tail 0.1对应z正值，下尾0.1对应负值。不要把density高度当probability。

##### 英文概念串联｜Connected explanation in English

A normal probability is an area under a continuous curve. In N(mu, sigma squared), the first parameter fixes the centre and the second parameter is the variance, so take its square root before standardising. A quick sketch should mark the mean, the boundary and the required tail; it provides an immediate check on whether the answer should be above or below one half.

##### 英文方法说明｜Method in English

Standardisation converts a distance from the mean into a number of standard deviations: z equals (x-mu)/sigma. In an inverse problem, first convert the stated tail to a cumulative probability, obtain the corresponding signed z-value, and then use x equals mu plus z sigma. The sign should agree with the boundary's position on the sketch.

#### 5.5.2 二项分布的正态近似｜Normal approximation to binomial

##### 知识点 01｜何时可用正态近似｜Conditions for the approximation

当n较大且p不过分接近0或1时，B(n,p)的柱状分布可用N(np,np(1-p))近似。常用检查是np和n(1-p)都足够大。

**English explanation.** Continuity correction aligns whole discrete bars with a continuous area. Write the original discrete event, the corrected continuous event and the approximating normal distribution so the logic is visible.

##### 知识点 02｜近似分布的均值与方差｜Parameters of the approximating normal

连续性修正把离散整数边界移0.5：P(X≤70)→P(Y<70.5)；P(X≥70)→P(Y>69.5)；P(60≤X≤70)→P(59.5<Y<70.5)。

##### 知识点 03｜连续性修正对应完整柱形｜Why continuity correction uses half-units

离散值70可想成覆盖69.5到70.5的柱。若连续曲线要包含整个“70”柱，边界必须放在70.5；这就是continuity correction，不是随意加减。

##### 知识点 04｜从离散事件到连续区间｜Translating the event before standardising

定义X~B(n,p)，检查条件；设Y~N(np,np(1-p))；翻译事件并做±0.5修正；标准化两个界值；算面积；写approximately。

##### 知识点 05｜单尾概率的完整近似｜A complete one-tail approximation

**题目｜Question.** X~B(200,0.4)，近似求P(X≤70)。

**正确答案｜Correct answer.** np=80，nq=120，条件合适。Y~N(80,48)。P(X≤70)≈P(Y<70.5)。z=(70.5-80)/√48≈-1.371，概率≈0.0851。

##### 知识点 06｜双边区间的连续性修正｜Correcting both ends of an interval

**题目｜Question.** 同一模型，近似求P(75≤X≤90)。

**正确答案｜Correct answer.** 修正为P(74.5<Y<90.5)。z1≈-0.794，z2≈1.516。概率=Φ(1.516)-Φ(-0.794)≈0.722。

##### 知识点 07｜条件不满足时不用近似｜Rejecting an unsuitable approximation

P(X≥70)使用69.5，不是70.5；“more than 70”是X≥71，修正同样为Y>70.5。若np或nq太小，正态形状可能很差。

##### 英文概念串联｜Connected explanation in English

A large binomial distribution can resemble a normal curve when both expected counts, np and nq, exceed 5. Use a new continuous variable Y with mean np and variance npq. Because this model replaces an exact discrete sum by a continuous area, the final probability is approximate even after a continuity correction.

##### 英文方法说明｜Method in English

Each integer value is represented by a unit-width bar centred on that integer. Therefore X at most k becomes Y below k+0.5, and X at least k becomes Y above k-0.5. Write the original discrete event, the corrected continuous event and the standardised z-value on separate lines; this makes the boundary logic visible and earns method credit.

### 三、核心词汇表｜Core vocabulary

- **normal distribution**｜正态分布：a continuous symmetric bell-shaped probability model
- **continuous random variable**｜连续随机变量：a variable taking any value in an interval
- **mean**｜均值：the centre and line of symmetry of a normal curve
- **variance**｜方差：the square of the standard deviation
- **standard deviation**｜标准差：the parameter controlling the spread of a normal curve
- **standard normal distribution**｜标准正态分布：the normal distribution with mean 0 and variance 1
- **standardise**｜标准化：convert X to Z by subtracting the mean and dividing by the standard deviation
- **z-value**｜标准分数：the number of standard deviations from the mean
- **lower tail**｜左尾：the area to the left of a boundary
- **upper tail**｜右尾：the area to the right of a boundary
- **central area**｜中央面积：the probability between two boundaries
- **symmetry**｜对称性：equal shape and area on opposite sides of the mean
- **percentile**｜百分位数：a boundary with a stated proportion below it
- **inverse normal**｜反求正态界值：finding a boundary from a stated cumulative probability
- **normal table**｜正态分布表：a table of cumulative standard-normal probabilities
- **probability density**｜概率密度：curve height whose interval area gives probability
- **normal approximation**｜正态近似：using a normal distribution in place of a binomial distribution
- **continuity correction**｜连续性修正：moving an integer boundary by 0.5 before a continuous approximation
- **approximating distribution**｜近似分布：the normal model N(np,npq) used for a binomial variable
- **inclusive boundary**｜包含端点：an endpoint whose whole discrete bar must be included
- **exclusive boundary**｜不包含端点：an endpoint excluded from the discrete event
- **discrete bar**｜离散柱：the unit-width bar centred on an integer value
- **approximately**｜近似等于：a label showing that one model has replaced another
- **parameter**｜参数：a value such as mean or variance defining the distribution
- **sketch**｜草图：a labelled curve showing the mean, boundary and required area

### 四、单元练习｜Unit practice（共 14 题）

#### 5.1 由草图检查尾部方向｜Checking the tail with a sketch

X~N(70,8²). Find P(X>82) with a sketch-based sign check.

#### 5.2 订正方差与标准差混用｜Correcting variance and standard deviation

For X~N(40,25), a student uses σ=25. Correct the calculation of P(X<45).

#### 5.3 由上尾概率反求界值｜Inverse normal from an upper tail

Find a such that P(X>a)=0.10 for X~N(100,12²), and explain the sign of z.

#### 5.4 选择与辨析｜Multiple choice

X~N(100,16). What is the standard deviation?
A 4  B 8  C 16  D 256

#### 5.5 结构化计算｜Structured calculation

X~N(80,25). Find P(72<X<88).

#### 5.6 迁移应用｜Transfer problem

Find the 95th percentile of N(40,6²).

#### 5.7 综合应用 2｜Extended application 2

Explain why standardisation uses (X−μ)/σ rather than (X−μ)/σ².

#### 5.8 写近似分布并修正边界｜Distribution and continuity correction

For X~B(120,0.4), write the approximating normal distribution and approximate P(X≤42).

#### 5.9 订正大于等于的边界｜Correcting a lower inclusive boundary

A student changes P(X≥70) to P(Y≥70.5). Correct the boundary and explain.

#### 5.10 检验近似条件｜Checking suitability

For X~B(50,0.04), evaluate whether a normal approximation is suitable.

#### 5.11 选择与辨析｜Multiple choice

Which is the corrected event for P(X<12)?
A Y<11.5  B Y<12  C Y<12.5  D Y>11.5

#### 5.12 结构化计算｜Structured calculation

Use a normal approximation for X~B(100,0.5) to find P(X≥60).

#### 5.13 迁移应用｜Transfer problem

Why must the final answer be labelled approximate?

#### 5.14 综合应用 2｜Extended application 2

Explain continuity correction for P(30≤X≤45) using discrete bars.

### 五、练习答案与解析｜Answers and explanations（共 14 题）

#### 5.1 由草图检查尾部方向｜Checking the tail with a sketch

**完整解答｜Full solution.** 82 is above the mean, so the required upper tail must be below 0.5. Standardise: z=(82−70)/8=1.5. Thus P(X>82)=P(Z>1.5)=1−Φ(1.5)=1−0.9332=0.0668.

#### 5.2 订正方差与标准差混用｜Correcting variance and standard deviation

**完整解答｜Full solution.** The second parameter is variance, so σ=√25=5. Then z=(45−40)/5=1 and P(X<45)=Φ(1)=0.8413. Using 25 confuses variance with standard deviation and gives the wrong scale.

#### 5.3 由上尾概率反求界值｜Inverse normal from an upper tail

**完整解答｜Full solution.** An upper-tail probability of 0.10 means a lies above the mean, so z is positive. Φ(z)=0.90 gives z≈1.2816. Therefore a=100+1.2816(12)≈115.4.

#### 5.4 选择与辨析｜Multiple choice

**完整解答｜Full solution.** A - 4, because the second parameter is variance and √16=4.

#### 5.5 结构化计算｜Structured calculation

**完整解答｜Full solution.** σ=5. z values are -1.6 and 1.6. Probability=P(-1.6<Z<1.6)=2Φ(1.6)-1≈0.890.

#### 5.6 迁移应用｜Transfer problem

**完整解答｜Full solution.** z0.95≈1.6449, so x=40+1.6449×6≈49.9.

#### 5.7 综合应用 2｜Extended application 2

**完整解答｜Full solution.** X−μ is a distance measured in the original units. Dividing by σ, which has the same units, produces a dimensionless number of standard deviations. Dividing by variance σ² would leave inverse units and would not create N(0,1).

#### 5.8 写近似分布并修正边界｜Distribution and continuity correction

**完整解答｜Full solution.** Mean=np=48; variance=np(1−p)=120(0.4)(0.6)=28.8. Let Y~N(48,28.8). Continuity correction changes X≤42 to Y<42.5. z=(42.5−48)/√28.8≈−1.025, so the probability is approximately Φ(−1.025)≈0.153.

#### 5.9 订正大于等于的边界｜Correcting a lower inclusive boundary

**完整解答｜Full solution.** X≥70 includes the entire bar centred at 70, whose lower edge is 69.5. The corrected event is therefore P(Y>69.5). Using 70.5 would omit the probability corresponding to X=70.

#### 5.10 检验近似条件｜Checking suitability

**完整解答｜Full solution.** np=50(0.04)=2 and n(1−p)=48. The first expected count is too small for a balanced bell shape, so a normal approximation is likely poor. An exact binomial calculation is preferable.

#### 5.11 选择与辨析｜Multiple choice

**完整解答｜Full solution.** A - X<12 means X≤11, so use Y<11.5.

#### 5.12 结构化计算｜Structured calculation

**完整解答｜Full solution.** Y~N(50,25). Correct to P(Y>59.5). z=(59.5-50)/5=1.9, so probability≈1-Φ(1.9)=0.0287.

#### 5.13 迁移应用｜Transfer problem

**完整解答｜Full solution.** A continuous normal area replaces a discrete binomial sum; even with correction the two distributions are not identical.

#### 5.14 综合应用 2｜Extended application 2

**完整解答｜Full solution.** Integer 30 is represented by the bar from 29.5 to 30.5, and integer 45 by the bar from 44.5 to 45.5. To include both complete end bars, the continuous event must be 29.5<Y<45.5.

### 六、自学检查清单｜Self-study checklist

- [ ] I can interpret the second parameter in N(mean, variance) as variance, not standard deviation.
- [ ] I can sketch a normal curve with the mean, boundary and required shaded area.
- [ ] I can standardise using Z=(X-mean)/standard deviation and show full working.
- [ ] I can use symmetry and complements for upper-tail and central probabilities.
- [ ] I can use an inverse normal value and choose the correct sign of z.
- [ ] I can find an unknown mean, standard deviation or boundary from a probability statement.
- [ ] I can check np>5 and nq>5 before using a normal approximation to a binomial variable.
- [ ] I can translate every common integer inequality to the correct half-unit boundary.
- [ ] I can label a normal-approximation answer as approximate and explain why.
