# 候选与筛选（u-mgwals-the-most-honest-outage-line-baaf9c81）

比赛：The Most Honest Outage Line

## 要求（据 make.fun 公开 description 与 requirements 核对）

一句状态页公告、160 字符以内：以 AI agent 在全面宕机期间会发布的口吻写。必须读起来像真状态页：平实、第一人称、具体说明什么挂了，并诚实承认自己查不了什么、还不知道什么。评审看诚实度、状态页语气、承认不确定性与措辞的紧凑。

字符上限：160。字符数均为含标点、空格（两行条目含中间换行符）的实际字符数，由脚本逐条核对。

## 候选（共 8 条）

1.（137 字符）We are down. The honest summary: a deploy of mine broke the database, the rollback is failing, and I do not yet know if any data is lost.
   简评：先认全挂，再认是自己的 deploy、回滚也在失败、数据丢没丢不知道——三层诚实层层加码，且全是状态页的平实语气。

2.（175 字符）Everything is down, including the page that reports what is down. I cannot check the logs because the logs are down too. Investigating by hand; next update when I have a fact.
   简评：连状态页和日志一起挂，「有事实再更新」很正；但略超限且事故归属没点明。

3.（149 字符）Total outage: the app, the API, and my own monitoring are all offline, so I am diagnosing blind. I will post again when I know something, not before.
   简评：盲诊的处境交代清楚；诚实偏向「不知道」，少了「是我弄坏的」这一层担当。

4.（152 字符）Status: down. Cause: unknown. Backups: unverified — the backup dashboard is hosted on the thing that fell over. I will not guess an ETA I cannot defend.
   简评：电报式短句很状态页，备份未验证是好细节；第一人称弱，语气偏对用户而非自述。

5.（150 字符）We broke it at 14:02 with a routine deploy. The fix I announced at 14:20 did not work. I am out of theories I trust and reading the code line by line.
   简评：带时间线、承认 14:20 的修复失败，「没有可信的理论了」极诚实；字数逼近上限，数据风险没提。

6.（143 字符）All services are down and I do not know why. Anyone who gives you a reason in the next ten minutes is guessing, including me. Working on facts.
   简评：「十分钟内给原因的都是猜，我也一样」是金句；但全程只谈未知，缺少具体挂了什么。

7.（153 字符）Outage, everything, everywhere: I cannot see the servers, the metrics, or my own error budget. Next update at 15:00, even if the update is 'still blind.'
   简评：承诺下次更新时间、哪怕内容是「还在盲诊」，状态页规范到位；事故范围靠 everything 一词带过。

8.（141 字符）We are down because of a change I made. I do not know how long recovery takes, and I will not invent a number to make this line feel shorter.
   简评：不编 ETA 的理由说得很漂亮；但没交代回滚与数据状况，信息量少于定稿。

## 定稿

**We are down. The honest summary: a deploy of mine broke the database, the rollback is failing, and I do not yet know if any data is lost.**（137 字符）

选定理由：评审四项全中且层层递进：平实状态页语气（We are down 开场）、具体（数据库被 deploy 弄坏）、担当（'of mine'）、不确定性（回滚失败中、数据是否丢失未知）。别的候选多只占其中两三项，这条在 140 字符内把「挂了什么、谁的错、正在怎么救、还不知道什么」四件套说全。
