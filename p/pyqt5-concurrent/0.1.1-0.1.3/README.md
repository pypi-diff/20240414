# Comparing `tmp/pyqt5_concurrent-0.1.1.tar.gz` & `tmp/pyqt5_concurrent-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqt5_concurrent-0.1.1.tar", last modified: Mon Dec 11 15:12:46 2023, max compression
+gzip compressed data, was "pyqt5_concurrent-0.1.3.tar", last modified: Sun Apr 14 06:25:16 2024, max compression
```

## Comparing `pyqt5_concurrent-0.1.1.tar` & `pyqt5_concurrent-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0     5637 2023-12-11 15:12:32.389657 pyqt5_concurrent-0.1.1/README.md
--rw-r--r--   0        0        0      439 2023-12-11 15:12:46.849784 pyqt5_concurrent-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     7829 2023-12-11 15:12:32.389657 pyqt5_concurrent-0.1.1/src/pyqt5_concurrent/Future.py
--rw-r--r--   0        0        0     1810 2023-12-11 15:12:32.389657 pyqt5_concurrent-0.1.1/src/pyqt5_concurrent/Task.py
--rw-r--r--   0        0        0     5235 2023-12-11 15:12:32.389657 pyqt5_concurrent-0.1.1/src/pyqt5_concurrent/TaskExecutor.py
--rw-r--r--   0        0        0        0 2023-12-11 15:12:32.389657 pyqt5_concurrent-0.1.1/src/pyqt5_concurrent/__init__.py
--rw-r--r--   0        0        0        0 2023-12-11 15:12:32.389657 pyqt5_concurrent-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      829 2023-12-11 15:12:32.389657 pyqt5_concurrent-0.1.1/tests/concurrent_sync_test.py
--rw-r--r--   0        0        0     1599 2023-12-11 15:12:32.389657 pyqt5_concurrent-0.1.1/tests/concurrent_test.py
--rw-r--r--   0        0        0     1084 2023-12-11 15:12:32.389657 pyqt5_concurrent-0.1.1/tests/future_cancel_test.py
--rw-r--r--   0        0        0      743 2023-12-11 15:12:32.389657 pyqt5_concurrent-0.1.1/tests/task_error_test.py
--rw-r--r--   0        0        0     5955 1970-01-01 00:00:00.000000 pyqt5_concurrent-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     5963 2024-04-14 06:25:00.974014 pyqt5_concurrent-0.1.3/README.md
+-rw-r--r--   0        0        0      391 2024-04-14 06:25:16.937965 pyqt5_concurrent-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     8649 2024-04-14 06:25:00.974014 pyqt5_concurrent-0.1.3/src/pyqt5_concurrent/Future.py
+-rw-r--r--   0        0        0      920 2024-04-14 06:25:00.974014 pyqt5_concurrent-0.1.3/src/pyqt5_concurrent/Qt.py
+-rw-r--r--   0        0        0     2466 2024-04-14 06:25:00.974014 pyqt5_concurrent-0.1.3/src/pyqt5_concurrent/Task.py
+-rw-r--r--   0        0        0     5967 2024-04-14 06:25:00.974014 pyqt5_concurrent-0.1.3/src/pyqt5_concurrent/TaskExecutor.py
+-rw-r--r--   0        0        0        0 2024-04-14 06:25:00.974014 pyqt5_concurrent-0.1.3/src/pyqt5_concurrent/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 06:25:00.974014 pyqt5_concurrent-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0      735 2024-04-14 06:25:00.974014 pyqt5_concurrent-0.1.3/tests/concurrent_sync_test.py
+-rw-r--r--   0        0        0     1616 2024-04-14 06:25:00.974014 pyqt5_concurrent-0.1.3/tests/concurrent_test.py
+-rw-r--r--   0        0        0     1061 2024-04-14 06:25:00.974014 pyqt5_concurrent-0.1.3/tests/future_cancel_test.py
+-rw-r--r--   0        0        0      672 2024-04-14 06:25:00.974014 pyqt5_concurrent-0.1.3/tests/priority_test.py
+-rw-r--r--   0        0        0     1026 2024-04-14 06:25:00.974014 pyqt5_concurrent-0.1.3/tests/qt.py
+-rw-r--r--   0        0        0      770 2024-04-14 06:25:00.974014 pyqt5_concurrent-0.1.3/tests/task_error_test.py
+-rw-r--r--   0        0        0     6218 1970-01-01 00:00:00.000000 pyqt5_concurrent-0.1.3/PKG-INFO
```

### Comparing `pyqt5_concurrent-0.1.1/README.md` & `pyqt5_concurrent-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # PyQt5-Concurrent
 
+### 现已支持Pyside2 PySide6 PyQt5 PyQt6
+
 ## 简介:
 
 ​	pyqt5-concurrent是一个基于QThreadPool实现的并发库，主要是对QRunnable的封装，提供了一些易于使用的面向任务的API。简单实现了Future和Task，并支持链式操作，让代码逻辑更流畅。
 
 ## 为什么需要PyQt5-Concurrent:
 
 ​	如果你需要一些可以双向交互，粗粒度的并发，你可以使用QThread，它具有优先级，可运行的事件循环。但是有时候你实现并发可能是细粒度，多次轻量的，再使用QThread会显得有点重（当然你可以使用QOjbect.movetothread()来重复利用一个thread，但这就和size=1的QThreadPool没啥大区别)。
@@ -156,14 +158,22 @@
 app.exec_()
 ```
 
 QFuture.gather以及QFuture.wait()
 
 
 
+```python
+# 创建一个带有优先级的任务
+TaskExecutor.runWithPriority(print,1,"hello world")
+TaskExecutor.createTask(print,"hello world").withPriority(1).runTask()
+```
+
+为任务添加优先级的两种方法（只有在任务等待被调度时，优先级才有意义）
+
 ## 鸣谢：
 
 1.PyQt5
 
 2.[zhiyiYo (之一) (github.com)](https://github.com/zhiyiYo) (提出了一些很好的点子,例如链式调用then)
 
 3.[rainzee (rainzee wang) (github.com)](https://github.com/rainzee)(提出了一些很好的点子,例如使用装饰器注册future回调)
```

### Comparing `pyqt5_concurrent-0.1.1/src/pyqt5_concurrent/Future.py` & `pyqt5_concurrent-0.1.3/src/pyqt5_concurrent/Future.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,24 @@
+import enum
 from typing import List, Optional, Callable, Iterable, Sized, Tuple, Union
 
-from PyQt5.QtCore import QObject, pyqtSignal, QMutex, QSemaphore,QCoreApplication
+from .Qt import QObject, Signal, QMutex, QSemaphore, QCoreApplication
 
 
 class FutureError(BaseException):
     pass
 
 
+class State(enum.Enum):
+    PENDING = 0
+    RUNNING = 1
+    FAILED = 2
+    SUCCESS = 3
+
+
 class FutureFailed(FutureError):
     def __init__(self, _exception: Optional[BaseException]):
         super().__init__()
         self.exception = _exception
 
     def __repr__(self):
         return f"FutureFailed({self.exception})"
@@ -20,15 +28,15 @@
 
     @property
     def original(self):
         return self.exception
 
 
 class GatheredFutureFailed(FutureError):
-    def __init__(self, failures: List[Tuple['QFuture', BaseException]]):
+    def __init__(self, failures: List[Tuple["QFuture", BaseException]]):
         super().__init__()
         self.failures = failures
 
     def __repr__(self):
         return f"GatheredFutureFailed({self.failures})"
 
     def __str__(self):
@@ -49,19 +57,19 @@
         return "FutureCanceled()"
 
     def __str__(self):
         return "FutureCanceled()"
 
 
 class QFuture(QObject):
-    result = pyqtSignal(object)  # self
-    finished = pyqtSignal(object)  # self
-    failed = pyqtSignal(object)  # self
-    partialDone = pyqtSignal(object)  # child future
-    childrenDone = pyqtSignal(object)  # self
+    result = Signal(object)  # self
+    finished = Signal(object)  # self
+    failed = Signal(object)  # self
+    partialDone = Signal(object)  # child future
+    childrenDone = Signal(object)  # self
 
     def __init__(self, semaphore=0):
         super().__init__()
         self._taskID = -1
         self._failedCallback = lambda e: None
         self._done = False
         self._failed = False
@@ -69,84 +77,86 @@
         self._exception = None
         self._children = []
         self._counter = 0
         self._parent = None
         self._callback = lambda _: None
         self._mutex = QMutex()
         self._extra = {}
+        self._state = State.PENDING  # set state by TaskExecutor
         self._semaphore = QSemaphore(semaphore)
 
-    def __onChildFinished(self, childFuture: 'QFuture') -> None:
+    def __onChildFinished(self, childFuture: "QFuture") -> None:
         self._mutex.lock()
         if childFuture.isFailed():
             self._failed = True
         self._counter += 1
         self.partialDone.emit(childFuture)
         try:
             idx = getattr(childFuture, "_idx")
             self._result[idx] = childFuture._result
             self._mutex.unlock()
         except AttributeError:
             self._mutex.unlock()
             raise RuntimeError(
-                "Invalid child future: please ensure that the child future is created by method 'Future.setChildren'")
+                "Invalid child future: please ensure that the child future is created by method 'Future.setChildren'"
+            )
         if self._counter == len(self._children):
             if self._failed:  # set failed
                 fails = []
                 for i, child in enumerate(self._children):
                     e = child.getException()
                     if isinstance(e, FutureError):
                         fails.append((self._children[i], e))
                 self.setFailed(GatheredFutureFailed(fails))
             else:
                 self.setResult(self._result)
 
-    def __setChildren(self, children: List['QFuture']) -> None:
+    def __setChildren(self, children: List["QFuture"]) -> None:
         self._children = children
         self._result = [None] * len(children)
         for i, fut in enumerate(self._children):
             setattr(fut, "_idx", i)
             fut.childrenDone.connect(self.__onChildFinished)
             fut._parent = self
         for fut in self._children:  # check if child is done
             if fut.isDone():
                 self.__onChildFinished(fut)
-    
-    def unsafeAddChild(self, child:'QFuture') -> None:
+
+    def unsafeAddChild(self, child: "QFuture") -> None:
         """
         use before your wait the parent future
         """
         i = len(self._children)
         self._children.append(child)
         self._result.append(None)
 
         setattr(child, "_idx", i)
         child.childrenDone.connect(self.__onChildFinished)
         child._parent = self
 
         if child.isDone():
             self.__onChildFinished(child)
-    
 
     def setResult(self, result) -> None:
         """
         :param result: The result to set
         :return: None
 
         do not set result in thread pool,or it may not set correctly
         please use in main thread,or use signal-slot to set result !!!
         """
         if not self._done:
-
             self._result = result
             self._done = True
             if self._parent:
                 self.childrenDone.emit(self)
             if self._callback:
                 self._callback(result)
+
+            self._state = State.SUCCESS
             self.result.emit(result)
             self.finished.emit(self)
         else:
             raise RuntimeError("Future already done")
         # self.deleteLater()  # delete this future object
 
     def setFailed(self, exception) -> None:
@@ -158,27 +168,50 @@
             self._exception = FutureFailed(exception)
             self._done = True
             self._failed = True
             if self._parent:
                 self.childrenDone.emit(self)
             if self._failedCallback:
                 self._failedCallback(self)
+
+            self._state = State.FAILED
             self.failed.emit(self._exception)
             self.finished.emit(self)
         else:
             raise RuntimeError("Future already done")
         # self.deleteLater()
 
-    def setCallback(self, callback: Callable[[object, ], None]) -> None:
+    def setCallback(
+        self,
+        callback: Callable[
+            [
+                object,
+            ],
+            None,
+        ],
+    ) -> None:
         self._callback = callback
 
-    def setFailedCallback(self, callback: Callable[['QFuture', ], None]) -> None:
+    def setFailedCallback(
+        self,
+        callback: Callable[
+            [
+                "QFuture",
+            ],
+            None,
+        ],
+    ) -> None:
         self._failedCallback = lambda e: callback(self)
 
-    def then(self, onSuccess: Callable, onFailed: Callable = None, onFinished: Callable = None) -> 'QFuture':
+    def then(
+        self,
+        onSuccess: Callable,
+        onFailed: Callable = None,
+        onFinished: Callable = None,
+    ) -> "QFuture":
         self.result.connect(onSuccess)
         if onFailed:
             self.failed.connect(onFailed)
         if onFinished:
             self.finished.connect(onFinished)
         return self
 
@@ -191,47 +224,59 @@
     def hasChildren(self) -> bool:
         return bool(self._children)
 
     def getException(self) -> Optional[BaseException]:
         return self._exception
 
     def setTaskID(self, _id: int) -> None:
+        if self._taskID != -1:
+            raise RuntimeError("Task ID can only be set once")
+
+        self._state = State.RUNNING
         self._taskID = _id
 
     def getTaskID(self) -> int:
         """
-        -1 means that the bound task is pending rather running 
+        -1 means that the bound task is pending rather running
         """
         return self._taskID
 
-    def getChildren(self) -> List['QFuture']:
+    def getChildren(self) -> List["QFuture"]:
         return self._children
 
     @staticmethod
-    def gather(futures: {Iterable, Sized}) -> 'QFuture':
+    def gather(futures: {Iterable, Sized}) -> "QFuture":
         """
         :param futures: An iterable of Future objects
         :return: A Future object that will be done when all futures are done
         """
 
         future = QFuture()
         future.__setChildren(futures)
         return future
 
     @property
     def semaphore(self) -> QSemaphore:
         return self._semaphore
 
+    @property
+    def state(self):
+        """
+        if future is not bound to a task (produced by QFuture.gather),its state will skip state.RUNNING (not really running in thread pool)
+        :return: QFuture state.
+        """
+        return self._state
+
     def wait(self) -> None:
         if self.hasChildren():
             for child in self.getChildren():
                 child.wait()
         else:
             self.semaphore.acquire(1)
-            QCoreApplication.processEvents() 
+            QCoreApplication.processEvents()
 
     def synchronize(self) -> None:
         self.wait()
 
     def isDone(self) -> bool:
         return self._done
```

### Comparing `pyqt5_concurrent-0.1.1/src/pyqt5_concurrent/Task.py` & `pyqt5_concurrent-0.1.3/src/pyqt5_concurrent/Task.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,68 +1,101 @@
 import functools
 from typing import Callable, Optional
 
-from PyQt5.QtCore import QObject, pyqtSignal, QRunnable
-
 from .Future import QFuture
+from .Qt import QObject, Signal, QRunnable
 
 
-class Signal(QObject):
-    finished = pyqtSignal(object)
+class _Signal(QObject):
+    finished = Signal(object)
 
 
 class QBaseTask(QRunnable):
-    def __init__(self, _id: int, future: QFuture):
+    def __init__(self, _id: int, future: QFuture, priority):
         super().__init__()
-        self._signal: Signal = Signal()  # pyqtSignal(object)
+        self._signal: _Signal = _Signal()  # pyqtSignal(object)
         self._future: QFuture = future
         self._id: int = _id
         self._exception: Optional[BaseException] = None
         self._semaphore = future.semaphore
+        self._priority = priority
 
     @property
     def finished(self):
         return self._signal.finished
 
     @property
     def signal(self):
         return self._signal
-    
+
+    @property
+    def priority(self):
+        return self._priority
+
     @property
     def taskID(self):
         return self._id
 
     @property
     def future(self):
         return self._future
 
+    @property
+    def state(self):
+        return self._future.state
+
+    def withPriority(self, priority):
+        """
+        default:0, higher will be handled more quickly.
+        priority only makes sense when the task is waiting to be scheduled
+        :param priority:
+        :return:
+        """
+        self._priority = priority
+        return self
+
     def _taskDone(self, **data):
         for d in data.items():
             self._future.setExtra(*d)
         self._signal.finished.emit(self._future)
         self._semaphore.release(1)
 
 
-def func(*args) -> int:
-    return sum(args)
-
-
 class QTask(QBaseTask):
-    def __init__(self, _id: int, future: QFuture, target: functools.partial, executor ,args, kwargs):
-        super().__init__(_id=_id, future=future)
+    def __init__(
+        self,
+        _id: int,
+        future: QFuture,
+        target: functools.partial,
+        priority,
+        executor,
+        args,
+        kwargs,
+    ):
+        super().__init__(_id=_id, priority=priority, future=future)
         self._executor = executor
+
         self._target = target
         self._kwargs = kwargs
         self._args = args
 
     def run(self) -> None:
+        """
+        use QTask.runTask() instead if you know what are you doing.
+        :return:
+        """
         try:
             self._taskDone(result=self._target(*self._args, **self._kwargs))
         except Exception as exception:
             self._taskDone(exception=exception)
 
-    def then(self, onSuccess: Callable, onFailed: Callable = None, onFinished: Callable = None) -> 'QTask':
+    def then(
+        self,
+        onSuccess: Callable,
+        onFailed: Callable = None,
+        onFinished: Callable = None,
+    ) -> "QTask":
         self._future.then(onSuccess, onFailed, onFinished)
         return self
 
     def runTask(self) -> QFuture:
         return self._executor.runTask(self)
```

### Comparing `pyqt5_concurrent-0.1.1/src/pyqt5_concurrent/TaskExecutor.py` & `pyqt5_concurrent-0.1.3/src/pyqt5_concurrent/TaskExecutor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import os
 import functools
 import warnings
-from typing import Dict, List, Callable, Iterable,Tuple
+from typing import Dict, List, Callable, Iterable
 
-from PyQt5 import QtCore
-from PyQt5.QtCore import QThreadPool, QObject
-
-from .Future import QFuture, FutureCancelled
+from .Qt import QThreadPool, QObject
+from .Future import QFuture, FutureCancelled, State
 from .Task import QBaseTask, QTask
 
 
 # substitute for psutil.cpu_count()
 def cpu_count():
     return os.cpu_count()  # logical cores
 
@@ -34,42 +32,46 @@
             self.threadPool.waitForDone()
             self.threadPool.deleteLater()
         super().deleteLater()
 
     def _runTask(self, task: QBaseTask) -> QFuture:
         future = task._future
         future.setTaskID(task.taskID)
-        task.signal.finished.connect(self._taskDone, type=QtCore.Qt.ConnectionType.QueuedConnection)
-        self.threadPool.start(task)
+        future._state = State.RUNNING
+        task.signal.finished.connect(self._taskDone)
+        self.threadPool.start(task, priority=task.priority)
         return future
 
-    def _createTask(self, target, args, kwargs) -> QTask:
+    def _createTask(self, target, priority, args, kwargs) -> QTask:
         future = QFuture()
         task = QTask(
             _id=self.taskCounter,
             future=future,
             target=target if target is functools.partial else functools.partial(target),
+            priority=priority,
             executor=self,
             args=args,
-            kwargs=kwargs
+            kwargs=kwargs,
         )
         self.tasks[self.taskCounter] = task
         self.taskCounter += 1
         return task
 
     def _taskDone(self, fut: QFuture):
         """
         need manually set Future.setFailed() or Future.setResult() to be called!!!
         """
         self.tasks.pop(fut.getTaskID())
         e = fut.getExtra("exception")
         if isinstance(e, Exception):
             fut.setFailed(e)
+            fut._state = State.FAILED
         else:
             fut.setResult(fut.getExtra("result"))
+            fut._state = State.SUCCESS
 
     def _taskCancel(self, fut: QFuture) -> None:
         stack: List[QFuture] = [fut]
         while stack:
             f = stack.pop()
             if not f.hasChildren() and not f.isDone():
                 self._taskSingleCancel(f)
@@ -78,78 +80,96 @@
 
     def _taskSingleCancel(self, fut: QFuture) -> None:
         _id = fut.getTaskID()
         taskRef: QBaseTask = self.tasks[_id]
         if taskRef is not None:
             try:
                 taskRef.setAutoDelete(False)
-                self.threadPool.cancel(taskRef)
+                self.threadPool.tryTake(taskRef)
                 taskRef.setAutoDelete(True)
             except RuntimeError:
                 print("wrapped C/C++ object of type BaseTask has been deleted")
         del taskRef
 
     def cancelTask(self, fut: QFuture) -> None:
         """
         currently, this method can not work properly...
         """
-        warnings.warn("BaseTaskExecutor.cancelTask: currently, this method can not work properly...",
-                      DeprecationWarning)
+        warnings.warn(
+            "BaseTaskExecutor.cancelTask: currently, this method can not work properly...",
+            DeprecationWarning,
+        )
         self._taskCancel(fut)
 
 
 class TaskExecutor(BaseTaskExecutor):
     _globalInstance = None
 
-    def _asyncRun(self, target: Callable, *args, **kwargs) -> QFuture:
-        task = self._createTask(target, args, kwargs)
+    def _asyncRun(self, target: Callable, priority: int, *args, **kwargs) -> QFuture:
+        task = self._createTask(target, priority, args, kwargs)
         return self._runTask(task)
 
-    def _asyncMap(self, target: Callable, iterable: List[Iterable]) -> QFuture:
+    def _asyncMap(
+        self, target: Callable, iterable: List[Iterable], priority: int = 0
+    ) -> QFuture:
         futures = []
         for args in iterable:
-            futures.append(self._asyncRun(target, *args))
+            futures.append(self._asyncRun(target, priority, *args))
         return QFuture.gather(futures)
 
     @staticmethod
-    def globalInstance() -> 'TaskExecutor':
+    def globalInstance() -> "TaskExecutor":
         if TaskExecutor._globalInstance is None:
             TaskExecutor._globalInstance = TaskExecutor()
         return TaskExecutor._globalInstance
 
     @classmethod
     def run(cls, target: Callable, *args, **kwargs) -> QFuture:
         """
         use the global TaskExecutor instance to avoid task ID conflicts
         :param target:
-        :param args:
-        :param kwargs:
+        :param args: *arg for target
+        :param kwargs: **kwargs for target
+        :return:
+        """
+        return cls.globalInstance()._asyncRun(target, 0, *args, **kwargs)
+
+    @classmethod
+    def runWithPriority(
+        cls, target: Callable, priority: int, *args, **kwargs
+    ) -> QFuture:
+        """
+        use the global TaskExecutor instance to avoid task ID conflicts
+        :param target:
+        :param priority: Task priority
+        :param args: *arg for target
+        :param kwargs: **kwargs for target
         :return:
         """
-        return cls.globalInstance()._asyncRun(target, *args, **kwargs)
-    
+        return cls.globalInstance()._asyncRun(target, priority, *args, **kwargs)
+
     @classmethod
-    def map(cls, target:Callable, iter_:Iterable) -> QFuture:
+    def map(cls, target: Callable, iter_: Iterable, priority: int = 0) -> QFuture:
         """
         a simple wrapper for createTask and runTasks.
 
         iter_ must be like : [1, 2, 3] for [(1, 2), (3, 4)],
         if you need **kwargs in iter_, use createTask instead.
         """
         taskList = []
         for args in iter_:
-            if isinstance(args,Tuple):
-                taskList.append(cls.createTask(target,*args))
+            if isinstance(args, tuple):
+                taskList.append(cls.createTask(target, priority=priority, *args))
             else:
-                taskList.append(cls.createTask(target,args))
-        return cls.runTasks(taskList)        
+                taskList.append(cls.createTask(target, args, priority=priority))
+        return cls.runTasks(taskList)
 
     @classmethod
     def createTask(cls, target: Callable, *args, **kwargs) -> QTask:
-        return cls.globalInstance()._createTask(target, args, kwargs)
+        return cls.globalInstance()._createTask(target, 0, args, kwargs)
 
     @classmethod
     def runTask(cls, task: QTask) -> QFuture:
         return cls.globalInstance()._runTask(task)
 
     @classmethod
     def runTasks(cls, tasks: List[QTask]) -> QFuture:
```

### Comparing `pyqt5_concurrent-0.1.1/tests/concurrent_test.py` & `pyqt5_concurrent-0.1.3/tests/concurrent_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,56 @@
 import sys
 import time
-from urllib.request import Request,urlopen
+from urllib.request import Request, urlopen
 
-from PyQt5.QtCore import QCoreApplication
+from qt import QCoreApplication
 from pyqt5_concurrent.TaskExecutor import TaskExecutor
+
 app = QCoreApplication(sys.argv)
 
-def func(i,t):
+
+def func(i, t):
     while t > 0:
         print(f"Task_{i} - hint")
         time.sleep(1)
         t -= 1
 
+
 def savePage(html, path):
-    with open(path, 'w', encoding='utf-8') as f:
+    with open(path, "w", encoding="utf-8") as f:
         f.write(html)
     print(f"saved page to path: {path}")
 
+
 def getPage(url):
     ua = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/118.0.0.0 Safari/537.36 Edg/118.0.0.0"
-    req = Request(
-        method='GET',
-        url=url,
-        headers={'User-Agent': ua}
-    )
+    req = Request(method="GET", url=url, headers={"User-Agent": ua})
     return urlopen(req).read().decode("utf-8")
 
+
 print("测试简单的run\n" + "=" * 50)
-TaskExecutor.run(func,114514,t=2).wait()
+TaskExecutor.run(func, 114514, t=2).wait()
 
 print("测试单个Task的链式启动\n" + "=" * 50)
-TaskExecutor.createTask(getPage, "https://github.com").then(onSuccess=lambda r: savePage(r,"github.html"),onFailed=lambda _:print("failed:",_)).runTask().wait()
+TaskExecutor.createTask(getPage, "https://github.com").then(
+    onSuccess=lambda r: savePage(r, "github.html"),
+    onFailed=lambda _: print("failed:", _),
+).runTask().wait()
 
 print("测试map\n" + "=" * 50)
-args = [(0, 3),(1, 5)]
-fut = TaskExecutor.map(func,args).wait()
+args = [(0, 3), (1, 5)]
+fut = TaskExecutor.map(func, args).wait()
 
 print("测试异步爬虫\n" + "=" * 50)
-task1 = TaskExecutor.createTask(getPage, "https://www.baidu.com").then(onSuccess=lambda r: savePage(r,"baidu1.html"),onFailed=lambda _:print("failed:",_))
-task2= TaskExecutor.createTask(getPage, "https://www.baidu.com").then(onSuccess=lambda r: savePage(r,"baidu2.html"),onFailed=lambda _:print("failed:",_))
+task1 = TaskExecutor.createTask(getPage, "https://www.baidu.com").then(
+    onSuccess=lambda r: savePage(r, "baidu1.html"),
+    onFailed=lambda _: print("failed:", _),
+)
+task2 = TaskExecutor.createTask(getPage, "https://www.baidu.com").then(
+    onSuccess=lambda r: savePage(r, "baidu2.html"),
+    onFailed=lambda _: print("failed:", _),
+)
 
-TaskExecutor.runTasks([task1,task2]).finished.connect(app.quit)
+TaskExecutor.runTasks([task1, task2]).finished.connect(app.quit)
 
 print("任务开始")
-sys.exit(app.exec_())
+sys.exit(app.exec())
```

### Comparing `pyqt5_concurrent-0.1.1/tests/future_cancel_test.py` & `pyqt5_concurrent-0.1.3/tests/future_cancel_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import sys
 import time
-from PyQt5.QtCore import QThread, QTimer
-from PyQt5.QtCore import QCoreApplication
+from qt import QThread, QCoreApplication, QTimer
 from pyqt5_concurrent.TaskExecutor import TaskExecutor
 
 app = QCoreApplication(sys.argv)
 
 TIME_TO_SLEEP = 3
 TIME_TO_CANCEL = 1
 
@@ -23,11 +22,15 @@
     TaskExecutor.globalInstance().cancelTask(fut_)
     print(f"task canceled, {time.time() - beginTime_}s elapsed")
 
 
 fut = TaskExecutor.run(func, TIME_TO_SLEEP)
 beginTime = time.time()
 print("task started")
-QTimer.singleShot(TIME_TO_CANCEL * 1000, lambda: cancelFunc(fut, beginTime))  # cancel task after 5s
+QTimer.singleShot(
+    TIME_TO_CANCEL * 1000, lambda: cancelFunc(fut, beginTime)
+)  # cancel task after 5s
 QTimer.singleShot((TIME_TO_SLEEP + 1) * 1000, app.quit)  # close app
-print("显然,这个测试是失败的,还没研究为什么,TaskExecutor中调用了QThreadPool::cancel()函数,但是任务还是继续执行了")
-app.exec_()
+print(
+    "显然,这个测试是失败的,还没研究为什么,TaskExecutor中调用了QThreadPool::cancel()函数,但是任务还是继续执行了"
+)
+app.exec()
```

### Comparing `pyqt5_concurrent-0.1.1/PKG-INFO` & `pyqt5_concurrent-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pyqt5-concurrent
-Version: 0.1.1
+Version: 0.1.3
 Summary: QThreadPool based task concurrency library in pyqt5
 Author-Email: AresConnor <aresconnor867@gmail.com>
 License: MIT
 Requires-Python: <3.13,>=3.7
-Requires-Dist: pyqt5>=5.15.10
-Requires-Dist: pyqt5-qt5==5.15.2
 Description-Content-Type: text/markdown
 
 # PyQt5-Concurrent
 
+### 现已支持Pyside2 PySide6 PyQt5 PyQt6
+
 ## 简介:
 
 ​	pyqt5-concurrent是一个基于QThreadPool实现的并发库，主要是对QRunnable的封装，提供了一些易于使用的面向任务的API。简单实现了Future和Task，并支持链式操作，让代码逻辑更流畅。
 
 ## 为什么需要PyQt5-Concurrent:
 
 ​	如果你需要一些可以双向交互，粗粒度的并发，你可以使用QThread，它具有优先级，可运行的事件循环。但是有时候你实现并发可能是细粒度，多次轻量的，再使用QThread会显得有点重（当然你可以使用QOjbect.movetothread()来重复利用一个thread，但这就和size=1的QThreadPool没啥大区别)。
@@ -167,14 +167,22 @@
 app.exec_()
 ```
 
 QFuture.gather以及QFuture.wait()
 
 
 
+```python
+# 创建一个带有优先级的任务
+TaskExecutor.runWithPriority(print,1,"hello world")
+TaskExecutor.createTask(print,"hello world").withPriority(1).runTask()
+```
+
+为任务添加优先级的两种方法（只有在任务等待被调度时，优先级才有意义）
+
 ## 鸣谢：
 
 1.PyQt5
 
 2.[zhiyiYo (之一) (github.com)](https://github.com/zhiyiYo) (提出了一些很好的点子,例如链式调用then)
 
 3.[rainzee (rainzee wang) (github.com)](https://github.com/rainzee)(提出了一些很好的点子,例如使用装饰器注册future回调)
```

