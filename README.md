<div class="Box-sc-g0xbh4-0 bJMeLZ js-snippet-clipboard-copy-unpositioned" data-hpc="true"><article class="markdown-body entry-content container-lg" itemprop="text"><div class="markdown-heading" dir="auto"><h1 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">OpenRAVE 的 UR5 控制器</font></font></h1><a id="user-content-ur5-controller-for-openrave" class="anchor" aria-label="永久链接：OpenRAVE 的 UR5 控制器" href="#ur5-controller-for-openrave"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto">
    <a target="_blank" rel="noopener noreferrer" href="https://github.com/roboticsleeds/ur5controller/blob/master/repo_assets/ridgeback_ur5_fts150_gripper.png"><img src="https://github.com/roboticsleeds/ur5controller/raw/master/repo_assets/ridgeback_ur5_fts150_gripper.png" width="250" style="max-width: 100%;"></a> 
    <a target="_blank" rel="noopener noreferrer" href="https://github.com/roboticsleeds/ur5controller/blob/master/repo_assets/ridgeback_ur5_gripper.png"><img src="https://github.com/roboticsleeds/ur5controller/raw/master/repo_assets/ridgeback_ur5_gripper.png" width="250" style="max-width: 100%;"></a> 
    <a target="_blank" rel="noopener noreferrer" href="https://github.com/roboticsleeds/ur5controller/blob/master/repo_assets/ridgeback_ur5.png"><img src="https://github.com/roboticsleeds/ur5controller/raw/master/repo_assets/ridgeback_ur5.png" width="250" style="max-width: 100%;"></a>
</p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">目前我们支持不同的型号（本项目中我们只提供UR5和二指机械手的控制器）：</font></font></p>
<ul dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Clearpath Ridgeback + UR5 + 力扭矩传感器 150 + RobotiQ 两指夹持器</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Clearpath Ridgeback + UR5 + RobotiQ 两指夹持器</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">克利尔帕斯脊背犬 + UR5</font></font></li>
</ul>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">该控制器将监听实时发布 UR5 机器人关节值的 ROS 主题，并在 OpenRAVE 中可视化 UR5 机器人的当前状态。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">该插件的另一个重要功能是能够在真实机器人上执行 OpenRAVE 规划器生成的轨迹。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">有一个测试程序演示了此功能，
</font></font><a href="/roboticsleeds/ur5controller/blob/master/scripts/control_ur5.py"><code>scripts/control_ur5</code></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在这种情况下，将在 OpenRAVE 中加载 UR5，然后让您控制桌子上方的 UR5 机器人（向左、向右、向前、向后移动以及顺时针和逆时针旋转夹具）。</font></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">1. 开发者和贡献者</font></font></h2><a id="user-content-1-developers-and-contributors" class="anchor" aria-label="永久链接： 1. 开发者和贡献者" href="#1-developers-and-contributors"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">UR5 OpenRAVE 控制器由利兹大学计算机学院</font></font><a href="https://artificial-intelligence.leeds.ac.uk/robot-manipulation/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">机器人操纵实验室</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">开发。</font></font></p>
<ul dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">作者：</font></font><a href="http://rpapallas.com" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">拉斐尔·帕帕拉斯</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">当前维护者：</font></font><a href="http://rpapallas.com" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Rafael Papallas</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></li>
</ul>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">2. 许可证</font></font></h2><a id="user-content-2-license" class="anchor" aria-label="永久链接：2. 许可证" href="#2-license"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">UR5 OpenRAVE 控制器根据 GNU 通用公共许可证 v3.0 获得许可。完整许可证可</font></font><a href="https://github.com/roboticsleeds/ur5controller/blob/master/LICENSE"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在此处</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">获取。</font></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">3. 包括</font></font></h2><a id="user-content-3-includes" class="anchor" aria-label="永久链接：3. 包括" href="#3-includes"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">该存储库包括以下内容：</font></font></p>
<ul dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">为 OpenRAVE 和 UR5 机器人定制的控制器。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">UR5 本身、Robotiq 二指夹具和 Clearpath Ridgeback 移动底座的 URDF 和 SRDF 文件。</font></font></li>
</ul>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">4. 安装</font></font></h2><a id="user-content-4-installation" class="anchor" aria-label="永久链接：4.安装" href="#4-installation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">您可以使用 Singularity 容器来获取此控制器，也可以通过在主机上将控制器构建为 catkin 包来获取此控制器。与在主机上构建相比，使用奇点容器的优势在于，您可以在主机上拥有不同的 Ubuntu 和 ROS 版本，并在运行 Ubuntu 14.04 和 ROS Indigo 的奇点容器中拥有 UR5 控制器。例如，您可以拥有一台运行 Ubuntu 18.04 的主机并使用 Singularity 容器运行 UR5 控制器。</font></font></p>
<details>
<summary><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">使用奇点容器</font></font></summary>
<br><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">
启动并运行此控制器的最简单方法是使用我们的 Singularity 容器。 
</font></font><ol dir="auto">
<li>Install Singularity on your machine by following <a href="https://www.sylabs.io/guides/3.0/user-guide/quick_start.html#quick-installation-steps" rel="nofollow">this</a>.</li>
<li>Then, follow the instructions from <a href="https://github.com/roboticsleeds/ur5controller_singularity">here</a>.</li>
</ol>
</details>
<details>
<summary><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在您自己的机器上从源代码构建</font></font></summary>
<br><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">
如果您希望在主机上构建此控件，您可以找到以下说明。
</font></font><div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto">Dependencies</h4><a id="user-content-dependencies" class="anchor" aria-label="Permalink: Dependencies" href="#dependencies"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul dir="auto">
<li><a href="https://github.com/ThomasTimm/ur_modern_driver">ur_modern_driver</a> needs to be installed on the computer that controls the robot and you need to run <code>roslaunch ur_modern_driver ur5_bringup.launch robot_ip:=THE_IP_OF_UR5_ROBOT</code>.</li>
<li>You need to install the <a href="https://github.com/personalrobotics/openrave_catkin">openrave_catkin</a>.</li>
<li>You need to install and configure another OpenRAVE plugin called <code>or_urdf</code> this plugin is available <a href="https://github.com/personalrobotics/or_urdf">here</a>. I have written a small guide on
how to install this plugin if you struggle to find a solution, find the tutorial <a href="https://gist.github.com/rpapallas/171cad0e881769647d0851b8780cc545">here</a>.</li>
<li><strong>(OPTIONAL)</strong> Install the Robotiq controller.
<ol dir="auto">
<li><code>cd ~/catkin_ws/src</code></li>
<li><code>git clone git@github.com:ros-industrial/robotiq.git</code></li>
<li><code>cd robotiq</code></li>
<li><code>git checkout indigo-devel</code></li>
<li><code>rosdep install robotiq_modbus_tcp</code></li>
<li><code>sudo apt-get install ros-indigo-soem</code></li>
<li><code>cd ~/catkin_ws</code></li>
<li><code>catkin_make</code></li>
</ol>
</li>
</ul>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto">Installation</h4><a id="user-content-installation" class="anchor" aria-label="Permalink: Installation" href="#installation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul dir="auto">
<li>Go to your catkin worksapce e.g <code>cd ~/catkin_ws/src</code> and clone this repository: <code>git clone git@github.com:roboticsleeds/ur5controller.git</code></li>
<li>Add the following line in your <code>~/.bashrc</code> file located under your home
directory by running the following command in the terminal: <code>echo  'export OPENRAVE_PLUGINS=$OPENRAVE_PLUGINS:~/catkin_ws/devel/share/openrave-0.9/plugins' &gt;&gt; ~/.bashrc</code></li>
<li>Run <code>source ~/.bashrc</code>.</li>
<li>Go to your catkin workspace <code>cd ~/catkin_ws</code> and run <code>catkin_make</code>. You should
see a successful message on build in which case you are ready to go. If you get
any errors at this stage, please review what went wrong.</li>
<li>Add in your <code>.bashrc</code> the Python path to the UR5 class by running</li>
</ul>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c1">echo</span> <span class="pl-s"><span class="pl-pds">'</span>export PYTHONPATH=$PYTHONPATH:~/catkin_ws/src/ur5controller/pythonsrc/ur5_robot<span class="pl-pds">'</span></span> <span class="pl-k">&gt;&gt;</span> <span class="pl-k">~</span>/.bashrc<span class="pl-s"><span class="pl-pds">`</span></span></pre><div class="zeroclipboard-container">
    
  </div></div>
<p dir="auto">This will let Python know where the Python classes for
creating UR5 robot instances in OpenRAVE are.</p>
</details>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">5. 测试控制器</font></font></h2><a id="user-content-5-testing-the-controller" class="anchor" aria-label="永久链接：5. 测试控制器" href="#5-testing-the-controller"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"></font><code>control_ur5.py</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">下面</font><font style="vertical-align: inherit;">有一个文件</font></font><code>scripts</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，您可以在真实的机器人上运行和测试控制器。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">有了 Python 类，在 OpenRAVE 中创建 UR5 机器人就变得非常简单：</font></font></p>
<details>
<summary><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">显示代码</font></font></summary>
<br>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-k">import</span> <span class="pl-v">IPython</span>
<span class="pl-k">from</span> <span class="pl-s1">ur5_factory</span> <span class="pl-k">import</span> <span class="pl-v">UR5_Factory</span>
<span class="pl-s1">ur5_factory</span> <span class="pl-c1">=</span> <span class="pl-v">UR5_Factory</span>()

<span class="pl-c"># If you want to specify all the configuration settings (is_simulation, has_ridgeback etc)</span>
<span class="pl-s1">env</span>, <span class="pl-s1">robot</span> <span class="pl-c1">=</span> <span class="pl-s1">ur5_factory</span>.<span class="pl-en">create_ur5_and_env</span>(<span class="pl-s1">is_simulation</span><span class="pl-c1">=</span><span class="pl-c1">True</span>,
                                            <span class="pl-s1">has_ridgeback</span><span class="pl-c1">=</span><span class="pl-c1">True</span>,
                                            <span class="pl-s1">gripper_name</span><span class="pl-c1">=</span><span class="pl-s">"robotiq_two_finger"</span>,
                                            <span class="pl-s1">has_force_torque_sensor</span><span class="pl-c1">=</span><span class="pl-c1">True</span>,
                                            <span class="pl-s1">env_path</span><span class="pl-c1">=</span><span class="pl-s">"test_env.xml"</span>,
                                            <span class="pl-s1">viewer_name</span><span class="pl-c1">=</span><span class="pl-s">"qtcoin"</span>,
                                            <span class="pl-s1">urdf_path</span><span class="pl-c1">=</span><span class="pl-s">"package://ur5controller/ur5_description/urdf/"</span>,
                                            <span class="pl-s1">srdf_path</span><span class="pl-c1">=</span><span class="pl-s">"package://ur5controller/ur5_description/srdf/"</span>)

<span class="pl-c"># The above is equivalent to the following (the `create_ur5_and_env` has set to defaults the values used above):</span>
<span class="pl-s1">env</span>, <span class="pl-s1">robot</span> <span class="pl-c1">=</span> <span class="pl-s1">ur5_factory</span>.<span class="pl-en">create_ur5_and_env</span>()
<span class="pl-v">IPython</span>.<span class="pl-en">embed</span>()</pre><div class="zeroclipboard-container">
   
  </div></div>
<p dir="auto">If you would like to use the model with no gripper, then you need to pass <code>None</code> to the <code>gripper_name</code> argument.</p>
</details>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">6. 控制器说明</font></font></h2><a id="user-content-6-controller-explained" class="anchor" aria-label="永久链接： 6. 控制器解释" href="#6-controller-explained"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ol dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">使用 URDF 插件在 OpenRAVE 中加载机器人：</font></font></li>
</ol>
<details>
<summary><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">显示代码</font></font></summary>
<br>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-k">import</span> <span class="pl-v">IPython</span>

<span class="pl-s1">env</span> <span class="pl-c1">=</span> <span class="pl-v">Environment</span>()
<span class="pl-s1">env</span>.<span class="pl-v">Load</span>(<span class="pl-s">'test_env.xml'</span>)
<span class="pl-s1">env</span>.<span class="pl-v">SetViewer</span>(<span class="pl-s">'qtcoin'</span>)

<span class="pl-s1">urdf_path</span> <span class="pl-c1">=</span> <span class="pl-s">"package://ur5controller/ur5_description/ur5.urdf"</span>
<span class="pl-s1">srdf_path</span> <span class="pl-c1">=</span> <span class="pl-s">"package://ur5controller/ur5_description/ur5.srdf"</span>

<span class="pl-s1">module</span> <span class="pl-c1">=</span> <span class="pl-v">RaveCreateModule</span>(<span class="pl-s1">env</span>, <span class="pl-s">'urdf'</span>)
<span class="pl-k">with</span> <span class="pl-s1">env</span>:
  <span class="pl-s1">name</span> <span class="pl-c1">=</span> <span class="pl-s1">module</span>.<span class="pl-v">SendCommand</span>(<span class="pl-s">'LoadURI {} {}'</span>.<span class="pl-en">format</span>(<span class="pl-s1">urdf_path</span>, <span class="pl-s1">srdf_path</span>))
  <span class="pl-s1">robot</span> <span class="pl-c1">=</span> <span class="pl-s1">env</span>.<span class="pl-v">GetRobot</span>(<span class="pl-s1">name</span>)

<span class="pl-s1">env</span>.<span class="pl-v">Add</span>(<span class="pl-s1">robot</span>, <span class="pl-c1">True</span>)</pre><div class="zeroclipboard-container">
    
  </div></div>
</details>
<ol start="2" dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">您现在需要使用</font></font><code>MultiController</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">.</font></font></li>
</ol>
<details>
<summary><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">显示代码</font></font></summary>
<br>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-s1">multicontroller</span> <span class="pl-c1">=</span> <span class="pl-v">RaveCreateMultiController</span>(<span class="pl-s1">env</span>, <span class="pl-s">""</span>)
<span class="pl-s1">robot</span>.<span class="pl-v">SetController</span>(<span class="pl-s1">multicontroller</span>)

<span class="pl-s1">robot_controller</span> <span class="pl-c1">=</span> <span class="pl-v">RaveCreateController</span>(<span class="pl-s1">env</span>,<span class="pl-s">'ur5controller'</span>)
<span class="pl-s1">hand_controller</span> <span class="pl-c1">=</span> <span class="pl-v">RaveCreateController</span>(<span class="pl-s1">env</span>, <span class="pl-s">'robotiqcontroller'</span>)

<span class="pl-s1">multicontroller</span>.<span class="pl-v">AttachController</span>(<span class="pl-s1">robot_controller</span>, [<span class="pl-c1">2</span>, <span class="pl-c1">1</span>, <span class="pl-c1">0</span>, <span class="pl-c1">4</span>, <span class="pl-c1">5</span>, <span class="pl-c1">6</span>], <span class="pl-c1">0</span>)
<span class="pl-s1">multicontroller</span>.<span class="pl-v">AttachController</span>(<span class="pl-s1">hand_controller</span>, [<span class="pl-c1">3</span>], <span class="pl-c1">0</span>)

<span class="pl-v">IPython</span>.<span class="pl-en">embed</span>()</pre><div class="zeroclipboard-container">
    
  </div></div>
<p dir="auto">You are now set. The OpenRAVE robot should update as you change the configuration
of the actual robot, and should also execute trajectories from OpenRAVE to
the actual robot.</p>
</details>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">七、其他注意事项</font></font></h2><a id="user-content-7-other-notes" class="anchor" aria-label="固定链接： 7. 其他注意事项" href="#7-other-notes"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<details>
<summary><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">检查用于连接控制器的 ROS 主题</font></font></summary>
<br>
<p dir="auto">This package will check (in ur5_factory.py) if certain topics are being published
(i.e <code>CModelRobotInput</code> and <code>CModelRobotOutput</code>) if you chose a gripper name
equal to "robotiq_two_finger_" and will not attach the corresponding controller
if those topics are not being published. This is a defensive mechanism to avoid
<code>IsDone()</code> method of the end-effector gripper returning false and blocking the
program execution. For more discussion, see <a href="https://stackoverflow.com/questions/49552755/openrave-controllerbase-is-blocking-at-the-isdone-method-and-never-returns/49552756#49552756" rel="nofollow">here</a></p>
</details>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">8. 故障排除</font></font></h2><a id="user-content-8-troubleshooting" class="anchor" aria-label="永久链接：8. 故障排除" href="#8-troubleshooting"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<details>
<summary><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">RuntimeError：调用 Python 对象时超出最大递归深度</font></font></summary>
<br>
<p dir="auto">If you get this error while the IK are being generated, then you probably have a version of sympy &gt; 0.7.1. Downgrade your sympy version to 0.7.1:</p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>pip install --upgrade sympy==0.7.1
</code></pre><div class="zeroclipboard-container">
    
  </div></div>
<p dir="auto">This should fix this issue.</p>
</details>
<details>
<summary><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">类型错误：“Poly”类型的参数不可迭代</font></font></summary>
<br>
<p dir="auto">If you get this error while the IK are being generated, then you probably have a version of sympy &gt; 0.7.1. Downgrade your sympy version to 0.7.1:</p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>pip install --upgrade sympy==0.7.1
</code></pre><div class="zeroclipboard-container">
   
  </div></div>
<p dir="auto">This should fix this issue.</p>
</details>
<details>
<summary><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在真实机器人上执行轨迹会导致意外动作</font></font></summary>
<br>
<p dir="auto"><strong>Issue:</strong> While OpenRAVE generates a trajectory that is smooth and valid in simulation during real execution the robot is strangely executing the trajectory.</p>
<p dir="auto"><strong>Possible solution:</strong> We came across this issue and the problem is probably down to the UR modern driver. When UR modern driver is installed using <code>apt-get</code> the problem appeared. The solution was to install UR modern driver as a catkin package (make sure to checkout the branch <code>kinetic-devel</code> although is kinetic is also working with indigo).</p>
</details>
</article></div>
