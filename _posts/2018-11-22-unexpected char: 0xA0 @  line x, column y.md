

---
layout: post
title:  "unexpected char: 0xA0 @  line X, column Y"
subtitle: ""
categories: ""
author: Geek
date:   2018-11-22 15:34:56 -0400
background: '/img/posts/01.jpg'
---

Error:
<br>
org.codehaus.groovy.control.MultipleCompilationErrorsException: startup failed:
script1542738817553815765628.groovy: 3: unexpected char: 0xA0 @ line 3, column 26.
def destinationPath = "*" + buildType + ".apk," + vars.getValue("nid") + ".apk";
^

1 error

    at org.codehaus.groovy.control.ErrorCollector.failIfErrors(ErrorCollector.java:302)
    at org.codehaus.groovy.control.ErrorCollector.addFatalError(ErrorCollector.java:149)
    at org.codehaus.groovy.control.ErrorCollector.addError(ErrorCollector.java:119)
    at org.codehaus.groovy.control.ErrorCollector.addError(ErrorCollector.java:131)
    at org.codehaus.groovy.control.SourceUnit.addError(SourceUnit.java:359)
    at org.codehaus.groovy.antlr.AntlrParserPlugin.transformCSTIntoAST(AntlrParserPlugin.java:137)
    at org.codehaus.groovy.antlr.AntlrParserPlugin.parseCST(AntlrParserPlugin.java:108)
    at org.codehaus.groovy.control.SourceUnit.parse(SourceUnit.java:236)
    at org.codehaus.groovy.control.CompilationUnit$1.call(CompilationUnit.java:161)
    at org.codehaus.groovy.control.CompilationUnit.applyToSourceUnits(CompilationUnit.java:846)
    at org.codehaus.groovy.control.CompilationUnit.doPhaseOperation(CompilationUnit.java:550)
    at org.codehaus.groovy.control.CompilationUnit.processPhaseOperations(CompilationUnit.java:526)
    at org.codehaus.groovy.control.CompilationUnit.compile(CompilationUnit.java:503)
    at groovy.lang.GroovyClassLoader.doParseClass(GroovyClassLoader.java:302)
    at groovy.lang.GroovyClassLoader.parseClass(GroovyClassLoader.java:281)
    at groovy.lang.GroovyClassLoader.parseClass(GroovyClassLoader.java:267)
    at groovy.lang.GroovyClassLoader.parseClass(GroovyClassLoader.java:214)
    at groovy.lang.GroovyClassLoader.parseClass(GroovyClassLoader.java:224)
    at com.pmease.quickbuild.plugin.basis.BasisPlugin$28.evaluate(BasisPlugin.java:321)
    at com.pmease.quickbuild.DefaultScriptEngine.evaluate(DefaultScriptEngine.java:81)
    at com.pmease.quickbuild.DefaultScriptEngine.interpolate(DefaultScriptEngine.java:105)
    at com.pmease.quickbuild.DefaultScriptEngine$Interpolator.intercept(DefaultScriptEngine.java:281)
    at com.pmease.quickbuild.plugin.artifact.ArtifactPublishStep$$EnhancerByCGLIB$$6ee94fd5.getFilePatterns(<generated>)
    at com.pmease.quickbuild.plugin.artifact.ArtifactPublishStep.run(ArtifactPublishStep.java:114)
    at com.pmease.quickbuild.plugin.artifact.ArtifactPublishStep$$EnhancerByCGLIB$$6ee94fd5.CGLIB$run$0(<generated>)
    at com.pmease.quickbuild.plugin.artifact.ArtifactPublishStep$$EnhancerByCGLIB$$6ee94fd5$$FastClassByCGLIB$$d1a7947b.invoke(<generated>)
    at net.sf.cglib.proxy.MethodProxy.invokeSuper(MethodProxy.java:215)
    at com.pmease.quickbuild.DefaultScriptEngine$Interpolator.intercept(DefaultScriptEngine.java:273)
    at com.pmease.quickbuild.plugin.artifact.ArtifactPublishStep$$EnhancerByCGLIB$$6ee94fd5.run(<generated>)
    at com.pmease.quickbuild.stepsupport.Step.execute(Step.java:539)
    at com.pmease.quickbuild.stepsupport.StepExecutionJob.executeStepAwareJob(StepExecutionJob.java:30)
    at com.pmease.quickbuild.stepsupport.StepAwareJob.executeBuildAwareJob(StepAwareJob.java:45)
    at com.pmease.quickbuild.BuildAwareJob.execute(BuildAwareJob.java:60)
    at com.pmease.quickbuild.grid.GridJob.run(GridJob.java:106)
    at java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:511)
    at java.util.concurrent.FutureTask.run(FutureTask.java:266)
    at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1142)
    at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:617)
    at java.lang.Thread.run(Thread.java:748)
    
<br>
    
    Reason: the spaces in the line are NO-BREAK SPACE. They should be SPACE.

<br>
How to fix:  change these NO-BREAK spaces to the correct SPACE ones.
