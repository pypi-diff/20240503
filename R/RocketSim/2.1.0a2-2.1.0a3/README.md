# Comparing `tmp/RocketSim-2.1.0a2.tar.gz` & `tmp/RocketSim-2.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RocketSim-2.1.0a2.tar", last modified: Thu Feb  8 03:22:57 2024, max compression
+gzip compressed data, was "RocketSim-2.1.0a3.tar", last modified: Fri May  3 02:02:44 2024, max compression
```

## Comparing `RocketSim-2.1.0a2.tar` & `RocketSim-2.1.0a3.tar`

### file list

```diff
@@ -1,331 +1,335 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.454495 RocketSim-2.1.0a2/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-08 03:22:57.454495 RocketSim-2.1.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.418491 RocketSim-2.1.0a2/RocketSim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-08 03:22:57.000000 RocketSim-2.1.0a2/RocketSim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    29310 2024-02-08 03:22:57.000000 RocketSim-2.1.0a2/RocketSim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 03:22:57.000000 RocketSim-2.1.0a2/RocketSim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-08 03:22:57.000000 RocketSim-2.1.0a2/RocketSim.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.414491 RocketSim-2.1.0a2/libsrc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.418491 RocketSim-2.1.0a2/libsrc/bullet3-3.24/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.414491 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.422492 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseProxy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseProxy.h
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)    37735 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvt.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    40585 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvt.h
--rw-r--r--   0 runner    (1001) docker     (127)    22805 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6622 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.h
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDispatcher.h
--rw-r--r--   0 runner    (1001) docker     (127)    17344 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13191 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.h
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCallback.h
--rw-r--r--   0 runner    (1001) docker     (127)    27531 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btQuantizedBvh.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    15084 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btQuantizedBvh.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.426492 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/
--rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/SphereTriangleDetector.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/SphereTriangleDetector.h
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btActivatingCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btActivatingCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)    22714 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxDetector.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxDetector.h
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionConfiguration.h
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionCreateFunc.h
--rw-r--r--   0 runner    (1001) docker     (127)    10605 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionDispatcher.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionDispatcher.h
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObject.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObject.h
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObjectWrapper.h
--rw-r--r--   0 runner    (1001) docker     (127)    48206 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionWorld.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    18241 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionWorld.h
--rw-r--r--   0 runner    (1001) docker     (127)    14945 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)    15777 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCompoundCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCompoundCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)    13862 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConcaveCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConcaveCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)    24106 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConvexAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConvexAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexPlaneCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexPlaneCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btDefaultCollisionConfiguration.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btDefaultCollisionConfiguration.h
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btEmptyCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btEmptyCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btGhostObject.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btGhostObject.h
--rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btHashedSimplePairCache.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btHashedSimplePairCache.h
--rw-r--r--   0 runner    (1001) docker     (127)    25716 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btInternalEdgeUtility.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btInternalEdgeUtility.h
--rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btManifoldResult.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btManifoldResult.h
--rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSimulationIslandManager.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSimulationIslandManager.h
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereBoxCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereBoxCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereSphereCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereSphereCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereTriangleCollisionAlgorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereTriangleCollisionAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btUnionFind.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btUnionFind.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.434493 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBoxShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7893 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBoxShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBvhTriangleMeshShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBvhTriangleMeshShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionMargin.h
--rw-r--r--   0 runner    (1001) docker     (127)     6042 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     8734 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCompoundShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCompoundShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConcaveShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConcaveShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexHullShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexHullShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexInternalShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexInternalShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexPolyhedron.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexPolyhedron.h
--rw-r--r--   0 runner    (1001) docker     (127)     9677 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btEmptyShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btEmptyShape.h
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btOptimizedBvh.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btOptimizedBvh.h
--rw-r--r--   0 runner    (1001) docker     (127)    14137 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btPolyhedralConvexShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btPolyhedralConvexShape.h
--rw-r--r--   0 runner    (1001) docker     (127)    25983 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btShapeHull.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btShapeHull.h
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btSphereShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btSphereShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStaticPlaneShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStaticPlaneShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStridingMeshInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStridingMeshInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTetrahedronShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTetrahedronShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleBuffer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleBuffer.h
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleCallback.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleCallback.h
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleIndexVertexArray.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleIndexVertexArray.h
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleInfoMap.h
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMesh.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMesh.h
--rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMeshShape.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMeshShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleShape.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.438493 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/
--rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btComputeGjkEpaPenetration.h
--rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btContinuousConvexCollision.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btContinuousConvexCollision.h
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexCast.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexCast.h
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexPenetrationDepthSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btDiscreteCollisionDetectorInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkCollisionDescription.h
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkConvexCast.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkConvexCast.h
--rw-r--r--   0 runner    (1001) docker     (127)    26341 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa2.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa2.h
--rw-r--r--   0 runner    (1001) docker     (127)    26567 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa3.h
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpaPenetrationDepthSolver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpaPenetrationDepthSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)    25685 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkPairDetector.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkPairDetector.h
--rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btManifoldPoint.h
--rw-r--r--   0 runner    (1001) docker     (127)    22069 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btMprPenetration.h
--rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPersistentManifold.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPersistentManifold.h
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPointCollector.h
--rw-r--r--   0 runner    (1001) docker     (127)    15895 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPolyhedralContactClipping.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPolyhedralContactClipping.h
--rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btRaycastCallback.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btRaycastCallback.h
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSimplexSolverInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSubSimplexConvexCast.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSubSimplexConvexCast.h
--rw-r--r--   0 runner    (1001) docker     (127)    17259 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btVoronoiSimplexSolver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btVoronoiSimplexSolver.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.414491 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.438493 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactConstraint.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactConstraint.h
--rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactSolverInfo.h
--rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btJacobianEntry.h
--rw-r--r--   0 runner    (1001) docker     (127)    86089 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSequentialImpulseConstraintSolver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSequentialImpulseConstraintSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSolverBody.h
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSolverConstraint.h
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btTypedConstraint.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11697 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btTypedConstraint.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.438493 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/Dynamics/
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btActionInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)    34628 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDiscreteDynamicsWorld.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDiscreteDynamicsWorld.h
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDynamicsWorld.h
--rw-r--r--   0 runner    (1001) docker     (127)    14866 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btRigidBody.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    19955 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btRigidBody.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.442494 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/Vehicle/
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btDefaultVehicleRaycaster.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btDefaultVehicleRaycaster.h
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btVehicleRaycaster.h
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btWheelInfo.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btWheelInfo.h
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.446494 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.446494 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/TaskScheduler/
--rw-r--r--   0 runner    (1001) docker     (127)    20707 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btTaskScheduler.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportPosix.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13419 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportWin32.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btAabbUtil2.h
--rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btAlignedAllocator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btAlignedAllocator.h
--rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btAlignedObjectArray.h
--rw-r--r--   0 runner    (1001) docker     (127)    28888 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btConvexHull.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btConvexHull.h
--rw-r--r--   0 runner    (1001) docker     (127)    56111 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btConvexHullComputer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btConvexHullComputer.h
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btCpuFeatureUtility.h
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btDefaultMotionState.h
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btGeometryUtil.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btGeometryUtil.h
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btGrahamScan2dConvexHull.h
--rw-r--r--   0 runner    (1001) docker     (127)     9560 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btHashMap.h
--rw-r--r--   0 runner    (1001) docker     (127)    24434 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btImplicitQRSVD.h
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btList.h
--rw-r--r--   0 runner    (1001) docker     (127)    43774 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btMatrix3x3.h
--rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btMatrixX.h
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btMinMax.h
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btModifiedGramSchmidt.h
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btMotionState.h
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btPolarDecomposition.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btPolarDecomposition.h
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btPoolAllocator.h
--rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btQuadWord.h
--rw-r--r--   0 runner    (1001) docker     (127)    29414 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btQuaternion.h
--rw-r--r--   0 runner    (1001) docker     (127)    22506 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btQuickprof.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btQuickprof.h
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btRandom.h
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btReducedVector.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btReducedVector.h
--rw-r--r--   0 runner    (1001) docker     (127)    24915 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btScalar.h
--rw-r--r--   0 runner    (1001) docker     (127)   128666 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btSerializer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    19953 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btSerializer.h
--rw-r--r--   0 runner    (1001) docker     (127)   128676 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btSerializer64.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13569 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btSpatialAlgebra.h
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btStackAlloc.h
--rw-r--r--   0 runner    (1001) docker     (127)    21959 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btThreads.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btThreads.h
--rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btTransform.h
--rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btTransformUtil.h
--rw-r--r--   0 runner    (1001) docker     (127)    57838 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btVector3.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    38269 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btVector3.h
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/btBulletCollisionCommon.h
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/libsrc/bullet3-3.24/btBulletDynamicsCommon.h
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.450495 RocketSim-2.1.0a2/python-mtheall/
--rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/python-mtheall/Angle.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    94546 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/python-mtheall/Arena.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/python-mtheall/Array.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/python-mtheall/Array.h
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/python-mtheall/Ball.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/python-mtheall/BallHitInfo.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13502 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/python-mtheall/BallState.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/python-mtheall/BoostPad.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/python-mtheall/BoostPadState.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13598 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/python-mtheall/Car.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    15026 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/python-mtheall/CarConfig.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/python-mtheall/CarControls.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    32069 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/python-mtheall/CarState.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/python-mtheall/DemoMode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/python-mtheall/GameMode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/python-mtheall/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/python-mtheall/MemoryWeightMode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/python-mtheall/Module.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    26199 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/python-mtheall/Module.h
--rw-r--r--   0 runner    (1001) docker     (127)    24671 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/python-mtheall/MutatorConfig.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/python-mtheall/PyRef.h
--rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/python-mtheall/RotMat.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/python-mtheall/Team.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/python-mtheall/Vec.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/python-mtheall/WheelPairConfig.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)     7834 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/python-mtheall/regression_test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    73088 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/python-mtheall/unit_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-08 03:22:57.454495 RocketSim-2.1.0a2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2568 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.450495 RocketSim-2.1.0a2/src/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/BaseInc.h
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/BulletLink.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/BulletLink.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.450495 RocketSim-2.1.0a2/src/CollisionMeshFile/
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/CollisionMeshFile/CollisionMeshFile.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/CollisionMeshFile/CollisionMeshFile.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.450495 RocketSim-2.1.0a2/src/DataStream/
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/DataStream/DataStreamIn.h
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/DataStream/DataStreamOut.h
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/DataStream/SerializeObject.h
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Framework.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.450495 RocketSim-2.1.0a2/src/Math/
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Math/Math.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Math/Math.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.450495 RocketSim-2.1.0a2/src/Math/MathTypes/
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Math/MathTypes/MathTypes.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Math/MathTypes/MathTypes.h
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/RLConst.h
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/RocketSim.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/RocketSim.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.454495 RocketSim-2.1.0a2/src/Sim/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.454495 RocketSim-2.1.0a2/src/Sim/Arena/
--rw-r--r--   0 runner    (1001) docker     (127)    34242 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Sim/Arena/Arena.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Sim/Arena/Arena.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.454495 RocketSim-2.1.0a2/src/Sim/Ball/
--rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Sim/Ball/Ball.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Sim/Ball/Ball.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.454495 RocketSim-2.1.0a2/src/Sim/BallHitInfo/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Sim/BallHitInfo/BallHitInfo.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Sim/BallHitInfo/BallHitInfo.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.454495 RocketSim-2.1.0a2/src/Sim/BallPredTracker/
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Sim/BallPredTracker/BallPredTracker.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Sim/BallPredTracker/BallPredTracker.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.454495 RocketSim-2.1.0a2/src/Sim/BoostPad/
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Sim/BoostPad/BoostPad.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Sim/BoostPad/BoostPad.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.454495 RocketSim-2.1.0a2/src/Sim/BoostPad/BoostPadGrid/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Sim/BoostPad/BoostPadGrid/BoostPadGrid.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Sim/BoostPad/BoostPadGrid/BoostPadGrid.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.454495 RocketSim-2.1.0a2/src/Sim/Car/
--rw-r--r--   0 runner    (1001) docker     (127)    27522 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Sim/Car/Car.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Sim/Car/Car.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.454495 RocketSim-2.1.0a2/src/Sim/Car/CarConfig/
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Sim/Car/CarConfig/CarConfig.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Sim/Car/CarConfig/CarConfig.h
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Sim/CarControls.h
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Sim/CollisionMasks.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.454495 RocketSim-2.1.0a2/src/Sim/GameEventTracker/
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Sim/GameEventTracker/GameEventTracker.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Sim/GameEventTracker/GameEventTracker.h
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Sim/GameMode.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.454495 RocketSim-2.1.0a2/src/Sim/MutatorConfig/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Sim/MutatorConfig/MutatorConfig.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Sim/MutatorConfig/MutatorConfig.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.454495 RocketSim-2.1.0a2/src/Sim/SuspensionCollisionGrid/
--rw-r--r--   0 runner    (1001) docker     (127)     7508 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Sim/SuspensionCollisionGrid/SuspensionCollisionGrid.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Sim/SuspensionCollisionGrid/SuspensionCollisionGrid.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 03:22:57.454495 RocketSim-2.1.0a2/src/Sim/btVehicleRL/
--rw-r--r--   0 runner    (1001) docker     (127)    14666 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Sim/btVehicleRL/btVehicleRL.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-02-08 03:22:51.000000 RocketSim-2.1.0a2/src/Sim/btVehicleRL/btVehicleRL.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.044651 RocketSim-2.1.0a3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-03 02:02:44.044651 RocketSim-2.1.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.008650 RocketSim-2.1.0a3/RocketSim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-03 02:02:43.000000 RocketSim-2.1.0a3/RocketSim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    29474 2024-05-03 02:02:43.000000 RocketSim-2.1.0a3/RocketSim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 02:02:43.000000 RocketSim-2.1.0a3/RocketSim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 02:02:43.000000 RocketSim-2.1.0a3/RocketSim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 02:02:43.000000 RocketSim-2.1.0a3/RocketSim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.000650 RocketSim-2.1.0a3/libsrc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.008650 RocketSim-2.1.0a3/libsrc/bullet3-3.24/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.000650 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.008650 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseProxy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseProxy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    37735 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvt.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    40585 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvt.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22805 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6622 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDispatcher.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17344 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13191 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCallback.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27531 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btQuantizedBvh.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15084 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btQuantizedBvh.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.016651 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/SphereTriangleDetector.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/SphereTriangleDetector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btActivatingCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btActivatingCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22714 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxDetector.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxDetector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionConfiguration.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionCreateFunc.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10605 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionDispatcher.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionDispatcher.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObject.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObject.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObjectWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)    48206 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionWorld.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18241 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionWorld.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14945 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15777 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCompoundCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCompoundCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13862 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConcaveCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConcaveCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24106 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConvexAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConvexAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexPlaneCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexPlaneCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btDefaultCollisionConfiguration.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btDefaultCollisionConfiguration.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btEmptyCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btEmptyCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btGhostObject.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btGhostObject.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btHashedSimplePairCache.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btHashedSimplePairCache.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25716 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btInternalEdgeUtility.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btInternalEdgeUtility.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btManifoldResult.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btManifoldResult.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14427 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSimulationIslandManager.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSimulationIslandManager.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereBoxCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereBoxCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereSphereCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereSphereCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereTriangleCollisionAlgorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereTriangleCollisionAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btUnionFind.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btUnionFind.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.020650 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBoxShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7893 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBoxShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBvhTriangleMeshShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBvhTriangleMeshShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionMargin.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6042 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8734 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCompoundShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCompoundShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConcaveShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConcaveShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexHullShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexHullShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexInternalShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexInternalShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexPolyhedron.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexPolyhedron.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9677 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btEmptyShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btEmptyShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btOptimizedBvh.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btOptimizedBvh.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14137 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btPolyhedralConvexShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btPolyhedralConvexShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25983 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btShapeHull.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btShapeHull.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btSphereShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btSphereShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStaticPlaneShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStaticPlaneShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStridingMeshInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStridingMeshInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTetrahedronShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTetrahedronShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleBuffer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleBuffer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleCallback.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleCallback.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleIndexVertexArray.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleIndexVertexArray.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleInfoMap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMesh.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMesh.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMeshShape.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMeshShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleShape.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.024651 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/
+-rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btComputeGjkEpaPenetration.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btContinuousConvexCollision.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btContinuousConvexCollision.h
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexCast.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexCast.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexPenetrationDepthSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btDiscreteCollisionDetectorInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkCollisionDescription.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkConvexCast.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkConvexCast.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26341 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa2.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa2.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26567 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa3.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpaPenetrationDepthSolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpaPenetrationDepthSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25685 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkPairDetector.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkPairDetector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btManifoldPoint.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22069 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btMprPenetration.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPersistentManifold.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPersistentManifold.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPointCollector.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15895 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPolyhedralContactClipping.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPolyhedralContactClipping.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btRaycastCallback.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btRaycastCallback.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSimplexSolverInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSubSimplexConvexCast.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSubSimplexConvexCast.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17259 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btVoronoiSimplexSolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btVoronoiSimplexSolver.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.000650 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.028651 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactConstraint.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactConstraint.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactSolverInfo.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btJacobianEntry.h
+-rw-r--r--   0 runner    (1001) docker     (127)    86089 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSequentialImpulseConstraintSolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSequentialImpulseConstraintSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSolverBody.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSolverConstraint.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btTypedConstraint.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11697 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btTypedConstraint.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.028651 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/Dynamics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btActionInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)    34628 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDiscreteDynamicsWorld.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDiscreteDynamicsWorld.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDynamicsWorld.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14866 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btRigidBody.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19955 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btRigidBody.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.028651 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/Vehicle/
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btDefaultVehicleRaycaster.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btDefaultVehicleRaycaster.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btVehicleRaycaster.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btWheelInfo.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btWheelInfo.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.032651 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.032651 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/TaskScheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)    20707 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btTaskScheduler.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportPosix.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13419 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportWin32.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btAabbUtil2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btAlignedAllocator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btAlignedAllocator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btAlignedObjectArray.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28888 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btConvexHull.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btConvexHull.h
+-rw-r--r--   0 runner    (1001) docker     (127)    56111 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btConvexHullComputer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btConvexHullComputer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btCpuFeatureUtility.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btDefaultMotionState.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btGeometryUtil.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btGeometryUtil.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btGrahamScan2dConvexHull.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9560 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btHashMap.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24434 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btImplicitQRSVD.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btList.h
+-rw-r--r--   0 runner    (1001) docker     (127)    43774 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btMatrix3x3.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btMatrixX.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btMinMax.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btModifiedGramSchmidt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btMotionState.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btPolarDecomposition.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btPolarDecomposition.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btPoolAllocator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btQuadWord.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29414 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btQuaternion.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22506 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btQuickprof.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btQuickprof.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btRandom.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btReducedVector.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btReducedVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24915 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btScalar.h
+-rw-r--r--   0 runner    (1001) docker     (127)   128666 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btSerializer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19953 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btSerializer.h
+-rw-r--r--   0 runner    (1001) docker     (127)   128676 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btSerializer64.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13569 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btSpatialAlgebra.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btStackAlloc.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21959 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btThreads.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btThreads.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btTransform.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btTransformUtil.h
+-rw-r--r--   0 runner    (1001) docker     (127)    57838 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btVector3.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    38269 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btVector3.h
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/btBulletCollisionCommon.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/libsrc/bullet3-3.24/btBulletDynamicsCommon.h
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.036651 RocketSim-2.1.0a3/python-mtheall/
+-rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/python-mtheall/Angle.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    94546 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/python-mtheall/Arena.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/python-mtheall/Array.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/python-mtheall/Array.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/python-mtheall/Ball.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11857 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/python-mtheall/BallHitInfo.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13522 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/python-mtheall/BallState.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/python-mtheall/BoostPad.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/python-mtheall/BoostPadState.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13598 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/python-mtheall/Car.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15053 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/python-mtheall/CarConfig.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/python-mtheall/CarControls.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    33997 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/python-mtheall/CarState.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/python-mtheall/DemoMode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/python-mtheall/GameMode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/python-mtheall/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/python-mtheall/MemoryWeightMode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/python-mtheall/Module.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    26961 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/python-mtheall/Module.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24676 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/python-mtheall/MutatorConfig.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/python-mtheall/PyRef.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10730 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/python-mtheall/RotMat.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/python-mtheall/Team.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/python-mtheall/Vec.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/python-mtheall/WheelPairConfig.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7834 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/python-mtheall/regression_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    73459 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/python-mtheall/unit_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 02:02:44.044651 RocketSim-2.1.0a3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2600 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.040651 RocketSim-2.1.0a3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/BaseInc.h
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/BulletLink.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/BulletLink.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.040651 RocketSim-2.1.0a3/src/CollisionMeshFile/
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/CollisionMeshFile/CollisionMeshFile.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/CollisionMeshFile/CollisionMeshFile.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.040651 RocketSim-2.1.0a3/src/DataStream/
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/DataStream/DataStreamIn.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/DataStream/DataStreamOut.h
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/DataStream/SerializeObject.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Framework.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.040651 RocketSim-2.1.0a3/src/Math/
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Math/Math.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Math/Math.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.040651 RocketSim-2.1.0a3/src/Math/MathTypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Math/MathTypes/MathTypes.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Math/MathTypes/MathTypes.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12048 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/RLConst.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/RocketSim.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/RocketSim.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.040651 RocketSim-2.1.0a3/src/Sim/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.040651 RocketSim-2.1.0a3/src/Sim/Arena/
+-rw-r--r--   0 runner    (1001) docker     (127)    34367 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/Arena/Arena.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/Arena/Arena.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.040651 RocketSim-2.1.0a3/src/Sim/Ball/
+-rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/Ball/Ball.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/Ball/Ball.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.040651 RocketSim-2.1.0a3/src/Sim/BallHitInfo/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/BallHitInfo/BallHitInfo.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/BallHitInfo/BallHitInfo.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.040651 RocketSim-2.1.0a3/src/Sim/BallPredTracker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/BallPredTracker/BallPredTracker.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/BallPredTracker/BallPredTracker.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.040651 RocketSim-2.1.0a3/src/Sim/BoostPad/
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/BoostPad/BoostPad.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/BoostPad/BoostPad.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.040651 RocketSim-2.1.0a3/src/Sim/BoostPad/BoostPadGrid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/BoostPad/BoostPadGrid/BoostPadGrid.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/BoostPad/BoostPadGrid/BoostPadGrid.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.040651 RocketSim-2.1.0a3/src/Sim/Car/
+-rw-r--r--   0 runner    (1001) docker     (127)    27775 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/Car/Car.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/Car/Car.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.040651 RocketSim-2.1.0a3/src/Sim/Car/CarConfig/
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/Car/CarConfig/CarConfig.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/Car/CarConfig/CarConfig.h
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/CarControls.h
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/CollisionMasks.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.040651 RocketSim-2.1.0a3/src/Sim/GameEventTracker/
+-rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/GameEventTracker/GameEventTracker.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/GameEventTracker/GameEventTracker.h
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/GameMode.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.040651 RocketSim-2.1.0a3/src/Sim/MutatorConfig/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/MutatorConfig/MutatorConfig.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/MutatorConfig/MutatorConfig.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.044651 RocketSim-2.1.0a3/src/Sim/PhysState/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/PhysState/PhysState.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/PhysState/PhysState.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.044651 RocketSim-2.1.0a3/src/Sim/SuspensionCollisionGrid/
+-rw-r--r--   0 runner    (1001) docker     (127)     7508 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/SuspensionCollisionGrid/SuspensionCollisionGrid.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/SuspensionCollisionGrid/SuspensionCollisionGrid.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:02:44.044651 RocketSim-2.1.0a3/src/Sim/btVehicleRL/
+-rw-r--r--   0 runner    (1001) docker     (127)    14699 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/btVehicleRL/btVehicleRL.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-05-03 02:02:37.000000 RocketSim-2.1.0a3/src/Sim/btVehicleRL/btVehicleRL.h
```

### Comparing `RocketSim-2.1.0a2/LICENSE` & `RocketSim-2.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/README.md` & `RocketSim-2.1.0a3/README.md`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/RocketSim.egg-info/SOURCES.txt` & `RocketSim-2.1.0a3/RocketSim.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -118,19 +118,21 @@
 /home/runner/work/RocketSim/RocketSim/src/Sim/BallPredTracker/BallPredTracker.cpp
 /home/runner/work/RocketSim/RocketSim/src/Sim/BoostPad/BoostPad.cpp
 /home/runner/work/RocketSim/RocketSim/src/Sim/BoostPad/BoostPadGrid/BoostPadGrid.cpp
 /home/runner/work/RocketSim/RocketSim/src/Sim/Car/Car.cpp
 /home/runner/work/RocketSim/RocketSim/src/Sim/Car/CarConfig/CarConfig.cpp
 /home/runner/work/RocketSim/RocketSim/src/Sim/GameEventTracker/GameEventTracker.cpp
 /home/runner/work/RocketSim/RocketSim/src/Sim/MutatorConfig/MutatorConfig.cpp
+/home/runner/work/RocketSim/RocketSim/src/Sim/PhysState/PhysState.cpp
 /home/runner/work/RocketSim/RocketSim/src/Sim/SuspensionCollisionGrid/SuspensionCollisionGrid.cpp
 /home/runner/work/RocketSim/RocketSim/src/Sim/btVehicleRL/btVehicleRL.cpp
 RocketSim.egg-info/PKG-INFO
 RocketSim.egg-info/SOURCES.txt
 RocketSim.egg-info/dependency_links.txt
+RocketSim.egg-info/requires.txt
 RocketSim.egg-info/top_level.txt
 libsrc/bullet3-3.24/LICENSE.txt
 libsrc/bullet3-3.24/MANIFEST.in
 libsrc/bullet3-3.24/README.md
 libsrc/bullet3-3.24/VERSION
 libsrc/bullet3-3.24/btBulletCollisionCommon.h
 libsrc/bullet3-3.24/btBulletDynamicsCommon.h
@@ -406,11 +408,13 @@
 src/Sim/Car/Car.h
 src/Sim/Car/CarConfig/CarConfig.cpp
 src/Sim/Car/CarConfig/CarConfig.h
 src/Sim/GameEventTracker/GameEventTracker.cpp
 src/Sim/GameEventTracker/GameEventTracker.h
 src/Sim/MutatorConfig/MutatorConfig.cpp
 src/Sim/MutatorConfig/MutatorConfig.h
+src/Sim/PhysState/PhysState.cpp
+src/Sim/PhysState/PhysState.h
 src/Sim/SuspensionCollisionGrid/SuspensionCollisionGrid.cpp
 src/Sim/SuspensionCollisionGrid/SuspensionCollisionGrid.h
 src/Sim/btVehicleRL/btVehicleRL.cpp
 src/Sim/btVehicleRL/btVehicleRL.h
```

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseInterface.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseInterface.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseProxy.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseProxy.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseProxy.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btBroadphaseProxy.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btCollisionAlgorithm.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btCollisionAlgorithm.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvt.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvt.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvt.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvt.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDbvtBroadphase.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDispatcher.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btDispatcher.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCache.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCallback.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btOverlappingPairCallback.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btQuantizedBvh.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btQuantizedBvh.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btQuantizedBvh.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/BroadphaseCollision/btQuantizedBvh.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/SphereTriangleDetector.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/SphereTriangleDetector.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/SphereTriangleDetector.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/SphereTriangleDetector.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btActivatingCollisionAlgorithm.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btActivatingCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btActivatingCollisionAlgorithm.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btActivatingCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxCollisionAlgorithm.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxCollisionAlgorithm.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxDetector.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxDetector.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxDetector.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btBoxBoxDetector.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionConfiguration.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionConfiguration.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionCreateFunc.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionCreateFunc.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionDispatcher.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionDispatcher.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionDispatcher.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionDispatcher.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObject.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObject.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObject.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObject.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObjectWrapper.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionObjectWrapper.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionWorld.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionWorld.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionWorld.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCollisionWorld.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCollisionAlgorithm.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCollisionAlgorithm.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCompoundCollisionAlgorithm.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCompoundCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCompoundCollisionAlgorithm.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btCompoundCompoundCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConcaveCollisionAlgorithm.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConcaveCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConcaveCollisionAlgorithm.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConcaveCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConvexAlgorithm.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConvexAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConvexAlgorithm.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexConvexAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexPlaneCollisionAlgorithm.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexPlaneCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexPlaneCollisionAlgorithm.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btConvexPlaneCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btDefaultCollisionConfiguration.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btDefaultCollisionConfiguration.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btDefaultCollisionConfiguration.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btDefaultCollisionConfiguration.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btEmptyCollisionAlgorithm.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btEmptyCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btEmptyCollisionAlgorithm.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btEmptyCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btGhostObject.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btGhostObject.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btGhostObject.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btGhostObject.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btHashedSimplePairCache.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btHashedSimplePairCache.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btHashedSimplePairCache.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btHashedSimplePairCache.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btInternalEdgeUtility.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btInternalEdgeUtility.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btInternalEdgeUtility.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btInternalEdgeUtility.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btManifoldResult.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btManifoldResult.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btManifoldResult.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btManifoldResult.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSimulationIslandManager.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSimulationIslandManager.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSimulationIslandManager.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSimulationIslandManager.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereBoxCollisionAlgorithm.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereBoxCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereBoxCollisionAlgorithm.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereBoxCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereSphereCollisionAlgorithm.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereSphereCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereSphereCollisionAlgorithm.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereSphereCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereTriangleCollisionAlgorithm.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereTriangleCollisionAlgorithm.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereTriangleCollisionAlgorithm.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btSphereTriangleCollisionAlgorithm.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btUnionFind.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btUnionFind.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btUnionFind.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionDispatch/btUnionFind.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBoxShape.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBoxShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBoxShape.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBoxShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBvhTriangleMeshShape.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBvhTriangleMeshShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBvhTriangleMeshShape.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBvhTriangleMeshShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionMargin.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionMargin.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionShape.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionShape.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCollisionShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCompoundShape.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCompoundShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCompoundShape.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCompoundShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConcaveShape.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConcaveShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConcaveShape.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConcaveShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexHullShape.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexHullShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexHullShape.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexHullShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexInternalShape.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexInternalShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexInternalShape.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexInternalShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexPolyhedron.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexPolyhedron.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexPolyhedron.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexPolyhedron.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexShape.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexShape.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btConvexShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btEmptyShape.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btEmptyShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btEmptyShape.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btEmptyShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btOptimizedBvh.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btOptimizedBvh.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btOptimizedBvh.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btOptimizedBvh.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btPolyhedralConvexShape.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btPolyhedralConvexShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btPolyhedralConvexShape.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btPolyhedralConvexShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btShapeHull.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btShapeHull.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btShapeHull.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btShapeHull.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btSphereShape.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btSphereShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btSphereShape.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btSphereShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStaticPlaneShape.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStaticPlaneShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStaticPlaneShape.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStaticPlaneShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStridingMeshInterface.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStridingMeshInterface.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStridingMeshInterface.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btStridingMeshInterface.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTetrahedronShape.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTetrahedronShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTetrahedronShape.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTetrahedronShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleBuffer.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleBuffer.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleBuffer.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleBuffer.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleCallback.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleCallback.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleCallback.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleCallback.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleIndexVertexArray.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleIndexVertexArray.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleIndexVertexArray.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleIndexVertexArray.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleInfoMap.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleInfoMap.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMesh.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMesh.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMesh.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMesh.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMeshShape.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMeshShape.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMeshShape.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleMeshShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleShape.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btTriangleShape.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btComputeGjkEpaPenetration.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btComputeGjkEpaPenetration.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btContinuousConvexCollision.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btContinuousConvexCollision.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btContinuousConvexCollision.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btContinuousConvexCollision.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexCast.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexCast.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexCast.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexCast.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexPenetrationDepthSolver.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btConvexPenetrationDepthSolver.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btDiscreteCollisionDetectorInterface.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btDiscreteCollisionDetectorInterface.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkCollisionDescription.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkCollisionDescription.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkConvexCast.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkConvexCast.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkConvexCast.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkConvexCast.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa2.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa2.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa2.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa2.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa3.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpa3.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpaPenetrationDepthSolver.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpaPenetrationDepthSolver.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpaPenetrationDepthSolver.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkEpaPenetrationDepthSolver.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkPairDetector.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkPairDetector.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkPairDetector.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btGjkPairDetector.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btManifoldPoint.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btManifoldPoint.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btMprPenetration.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btMprPenetration.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPersistentManifold.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPersistentManifold.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPersistentManifold.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPersistentManifold.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPointCollector.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPointCollector.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPolyhedralContactClipping.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPolyhedralContactClipping.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPolyhedralContactClipping.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btPolyhedralContactClipping.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btRaycastCallback.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btRaycastCallback.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btRaycastCallback.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btRaycastCallback.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSimplexSolverInterface.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSimplexSolverInterface.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSubSimplexConvexCast.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSubSimplexConvexCast.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSubSimplexConvexCast.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btSubSimplexConvexCast.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btVoronoiSimplexSolver.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btVoronoiSimplexSolver.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btVoronoiSimplexSolver.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletCollision/NarrowPhaseCollision/btVoronoiSimplexSolver.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactConstraint.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactConstraint.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactConstraint.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactConstraint.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactSolverInfo.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btContactSolverInfo.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btJacobianEntry.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btJacobianEntry.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSequentialImpulseConstraintSolver.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSequentialImpulseConstraintSolver.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSequentialImpulseConstraintSolver.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSequentialImpulseConstraintSolver.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSolverBody.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSolverBody.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSolverConstraint.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btSolverConstraint.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btTypedConstraint.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btTypedConstraint.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btTypedConstraint.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/ConstraintSolver/btTypedConstraint.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btActionInterface.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btActionInterface.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDiscreteDynamicsWorld.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDiscreteDynamicsWorld.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDiscreteDynamicsWorld.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDiscreteDynamicsWorld.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDynamicsWorld.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btDynamicsWorld.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btRigidBody.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btRigidBody.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btRigidBody.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/Dynamics/btRigidBody.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btDefaultVehicleRaycaster.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btDefaultVehicleRaycaster.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btDefaultVehicleRaycaster.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btDefaultVehicleRaycaster.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btVehicleRaycaster.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btVehicleRaycaster.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btWheelInfo.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btWheelInfo.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btWheelInfo.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/BulletDynamics/Vehicle/btWheelInfo.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LICENSE.txt` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btTaskScheduler.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btTaskScheduler.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportInterface.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportInterface.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportPosix.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportPosix.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportWin32.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/TaskScheduler/btThreadSupportWin32.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btAabbUtil2.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btAabbUtil2.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btAlignedAllocator.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btAlignedAllocator.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btAlignedAllocator.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btAlignedAllocator.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btAlignedObjectArray.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btAlignedObjectArray.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btConvexHull.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btConvexHull.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btConvexHull.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btConvexHull.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btConvexHullComputer.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btConvexHullComputer.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btConvexHullComputer.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btConvexHullComputer.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btCpuFeatureUtility.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btCpuFeatureUtility.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btDefaultMotionState.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btDefaultMotionState.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btGeometryUtil.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btGeometryUtil.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btGeometryUtil.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btGeometryUtil.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btGrahamScan2dConvexHull.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btGrahamScan2dConvexHull.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btHashMap.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btHashMap.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btImplicitQRSVD.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btImplicitQRSVD.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btList.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btList.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btMatrix3x3.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btMatrix3x3.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btMatrixX.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btMatrixX.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btMinMax.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btMinMax.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btModifiedGramSchmidt.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btModifiedGramSchmidt.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btMotionState.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btMotionState.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btPolarDecomposition.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btPolarDecomposition.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btPolarDecomposition.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btPolarDecomposition.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btPoolAllocator.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btPoolAllocator.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btQuadWord.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btQuadWord.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btQuaternion.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btQuaternion.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btQuickprof.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btQuickprof.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btQuickprof.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btQuickprof.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btRandom.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btRandom.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btReducedVector.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btReducedVector.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btReducedVector.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btReducedVector.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btScalar.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btScalar.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btSerializer.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btSerializer.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btSerializer.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btSerializer.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btSerializer64.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btSerializer64.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btSpatialAlgebra.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btSpatialAlgebra.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btStackAlloc.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btStackAlloc.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btThreads.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btThreads.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btThreads.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btThreads.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btTransform.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btTransform.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btTransformUtil.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btTransformUtil.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btVector3.cpp` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btVector3.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/LinearMath/btVector3.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/LinearMath/btVector3.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/MANIFEST.in` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/README.md` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/README.md`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/btBulletCollisionCommon.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/btBulletCollisionCommon.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/libsrc/bullet3-3.24/btBulletDynamicsCommon.h` & `RocketSim-2.1.0a3/libsrc/bullet3-3.24/btBulletDynamicsCommon.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/python-mtheall/Angle.cpp` & `RocketSim-2.1.0a3/python-mtheall/Angle.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/python-mtheall/Arena.cpp` & `RocketSim-2.1.0a3/python-mtheall/Arena.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/python-mtheall/Array.cpp` & `RocketSim-2.1.0a3/python-mtheall/Array.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/python-mtheall/Array.h` & `RocketSim-2.1.0a3/python-mtheall/Array.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/python-mtheall/Ball.cpp` & `RocketSim-2.1.0a3/python-mtheall/Ball.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/python-mtheall/BallHitInfo.cpp` & `RocketSim-2.1.0a3/python-mtheall/BallHitInfo.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -297,15 +297,15 @@
 }
 
 int BallHitInfo::Setrelative_pos_on_ball (BallHitInfo *self_, PyObject *value_, void *) noexcept
 {
 	if (!value_)
 	{
 		PyErr_SetString (
-		    PyExc_TypeError, "can't delete 'relative_pos_on_ball' attribute of 'RocketSim.BallHitInfo' objects");
+		    PyExc_AttributeError, "can't delete 'relative_pos_on_ball' attribute of 'RocketSim.BallHitInfo' objects");
 		return -1;
 	}
 
 	if (!Py_IS_TYPE (value_, Vec::Type))
 	{
 		PyErr_SetString (PyExc_TypeError, "attribute value type must be RocketSim.Vec");
 		return -1;
@@ -324,15 +324,15 @@
 	return PyRef<Vec>::incRef (self_->ballPos).giftObject ();
 }
 
 int BallHitInfo::Setball_pos (BallHitInfo *self_, PyObject *value_, void *) noexcept
 {
 	if (!value_)
 	{
-		PyErr_SetString (PyExc_TypeError, "can't delete 'ball_pos' attribute of 'RocketSim.BallHitInfo' objects");
+		PyErr_SetString (PyExc_AttributeError, "can't delete 'ball_pos' attribute of 'RocketSim.BallHitInfo' objects");
 		return -1;
 	}
 
 	if (!Py_IS_TYPE (value_, Vec::Type))
 	{
 		PyErr_SetString (PyExc_TypeError, "attribute value type must be RocketSim.Vec");
 		return -1;
@@ -348,15 +348,16 @@
 	return PyRef<Vec>::incRef (self_->extraHitVel).giftObject ();
 }
 
 int BallHitInfo::Setextra_hit_vel (BallHitInfo *self_, PyObject *value_, void *) noexcept
 {
 	if (!value_)
 	{
-		PyErr_SetString (PyExc_TypeError, "can't delete 'extra_hit_vel' attribute of 'RocketSim.BallHitInfo' objects");
+		PyErr_SetString (
+		    PyExc_AttributeError, "can't delete 'extra_hit_vel' attribute of 'RocketSim.BallHitInfo' objects");
 		return -1;
 	}
 
 	if (!Py_IS_TYPE (value_, Vec::Type))
 	{
 		PyErr_SetString (PyExc_TypeError, "attribute value type must be RocketSim.Vec");
 		return -1;
```

### Comparing `RocketSim-2.1.0a2/python-mtheall/BallState.cpp` & `RocketSim-2.1.0a3/python-mtheall/BallState.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -341,15 +341,15 @@
 	return PyRef<Vec>::incRef (self_->pos).giftObject ();
 }
 
 int BallState::Setpos (BallState *self_, PyObject *value_, void *) noexcept
 {
 	if (!value_)
 	{
-		PyErr_SetString (PyExc_TypeError, "can't delete 'pos' attribute of 'RocketSim.BallState' objects");
+		PyErr_SetString (PyExc_AttributeError, "can't delete 'pos' attribute of 'RocketSim.BallState' objects");
 		return -1;
 	}
 
 	if (!Py_IS_TYPE (value_, Vec::Type))
 	{
 		PyErr_SetString (PyExc_TypeError, "attribute value type must be RocketSim.Vec");
 		return -1;
@@ -368,15 +368,15 @@
 	return PyRef<RotMat>::incRef (self_->rotMat).giftObject ();
 }
 
 int BallState::Setrot_mat (BallState *self_, PyObject *value_, void *) noexcept
 {
 	if (!value_)
 	{
-		PyErr_SetString (PyExc_TypeError, "can't delete 'rot_mat' attribute of 'RocketSim.BallState' objects");
+		PyErr_SetString (PyExc_AttributeError, "can't delete 'rot_mat' attribute of 'RocketSim.BallState' objects");
 		return -1;
 	}
 
 	if (!Py_IS_TYPE (value_, RotMat::Type))
 	{
 		PyErr_SetString (PyExc_TypeError, "attribute value type must be RocketSim.RotMat");
 		return -1;
@@ -392,15 +392,15 @@
 	return PyRef<Vec>::incRef (self_->vel).giftObject ();
 }
 
 int BallState::Setvel (BallState *self_, PyObject *value_, void *) noexcept
 {
 	if (!value_)
 	{
-		PyErr_SetString (PyExc_TypeError, "can't delete 'vel' attribute of 'RocketSim.BallState' objects");
+		PyErr_SetString (PyExc_AttributeError, "can't delete 'vel' attribute of 'RocketSim.BallState' objects");
 		return -1;
 	}
 
 	if (!Py_IS_TYPE (value_, Vec::Type))
 	{
 		PyErr_SetString (PyExc_TypeError, "attribute value type must be RocketSim.Vec");
 		return -1;
@@ -416,15 +416,15 @@
 	return PyRef<Vec>::incRef (self_->angVel).giftObject ();
 }
 
 int BallState::Setang_vel (BallState *self_, PyObject *value_, void *) noexcept
 {
 	if (!value_)
 	{
-		PyErr_SetString (PyExc_TypeError, "can't delete 'ang_vel' attribute of 'RocketSim.BallState' objects");
+		PyErr_SetString (PyExc_AttributeError, "can't delete 'ang_vel' attribute of 'RocketSim.BallState' objects");
 		return -1;
 	}
 
 	if (!Py_IS_TYPE (value_, Vec::Type))
 	{
 		PyErr_SetString (PyExc_TypeError, "attribute value type must be RocketSim.Vec");
 		return -1;
```

### Comparing `RocketSim-2.1.0a2/python-mtheall/BoostPad.cpp` & `RocketSim-2.1.0a3/python-mtheall/BoostPad.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/python-mtheall/BoostPadState.cpp` & `RocketSim-2.1.0a3/python-mtheall/BoostPadState.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/python-mtheall/Car.cpp` & `RocketSim-2.1.0a3/python-mtheall/Car.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/python-mtheall/CarConfig.cpp` & `RocketSim-2.1.0a3/python-mtheall/CarConfig.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -402,15 +402,15 @@
 	return PyRef<Vec>::incRef (self_->hitboxSize).giftObject ();
 }
 
 int CarConfig::Sethitbox_size (CarConfig *self_, PyObject *value_, void *) noexcept
 {
 	if (!value_)
 	{
-		PyErr_SetString (PyExc_TypeError, "can't delete 'hitbox_size' attribute of 'RocketSim.CarConfig' objects");
+		PyErr_SetString (PyExc_AttributeError, "can't delete 'hitbox_size' attribute of 'RocketSim.CarConfig' objects");
 		return -1;
 	}
 
 	if (!Py_IS_TYPE (value_, Vec::Type))
 	{
 		PyErr_SetString (PyExc_TypeError, "attribute value type must be RocketSim.Vec");
 		return -1;
@@ -427,15 +427,15 @@
 }
 
 int CarConfig::Sethitbox_pos_offset (CarConfig *self_, PyObject *value_, void *) noexcept
 {
 	if (!value_)
 	{
 		PyErr_SetString (
-		    PyExc_TypeError, "can't delete 'hitbox_pos_offset' attribute of 'RocketSim.CarConfig' objects");
+		    PyExc_AttributeError, "can't delete 'hitbox_pos_offset' attribute of 'RocketSim.CarConfig' objects");
 		return -1;
 	}
 
 	if (!Py_IS_TYPE (value_, Vec::Type))
 	{
 		PyErr_SetString (PyExc_TypeError, "attribute value type must be RocketSim.Vec");
 		return -1;
@@ -451,15 +451,16 @@
 	return PyRef<WheelPairConfig>::incRef (self_->frontWheels).giftObject ();
 }
 
 int CarConfig::Setfront_wheels (CarConfig *self_, PyObject *value_, void *) noexcept
 {
 	if (!value_)
 	{
-		PyErr_SetString (PyExc_TypeError, "can't delete 'front_wheels' attribute of 'RocketSim.CarConfig' objects");
+		PyErr_SetString (
+		    PyExc_AttributeError, "can't delete 'front_wheels' attribute of 'RocketSim.CarConfig' objects");
 		return -1;
 	}
 
 	if (!Py_IS_TYPE (value_, WheelPairConfig::Type))
 	{
 		PyErr_SetString (PyExc_TypeError, "attribute value type must be RocketSim.WheelPairConfig");
 		return -1;
@@ -475,15 +476,15 @@
 	return PyRef<WheelPairConfig>::incRef (self_->backWheels).giftObject ();
 }
 
 int CarConfig::Setback_wheels (CarConfig *self_, PyObject *value_, void *) noexcept
 {
 	if (!value_)
 	{
-		PyErr_SetString (PyExc_TypeError, "can't delete 'back_wheels' attribute of 'RocketSim.CarConfig' objects");
+		PyErr_SetString (PyExc_AttributeError, "can't delete 'back_wheels' attribute of 'RocketSim.CarConfig' objects");
 		return -1;
 	}
 
 	if (!Py_IS_TYPE (value_, WheelPairConfig::Type))
 	{
 		PyErr_SetString (PyExc_TypeError, "attribute value type must be RocketSim.WheelPairConfig");
 		return -1;
```

### Comparing `RocketSim-2.1.0a2/python-mtheall/CarControls.cpp` & `RocketSim-2.1.0a3/python-mtheall/CarControls.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/python-mtheall/CarState.cpp` & `RocketSim-2.1.0a3/python-mtheall/CarState.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 #include "Module.h"
 
+#include <algorithm>
 #include <cstddef>
 #include <cstring>
 
 namespace RocketSim::Python
 {
+constexpr unsigned NUM_WHEELS = std::extent_v<decltype (RocketSim::CarState::wheelsWithContact)>;
+
 PyTypeObject *CarState::Type = nullptr;
 
 PyMemberDef CarState::Members[] = {
     {.name      = "update_counter",
         .type   = TypeHelper<decltype (RocketSim::CarState::updateCounter)>::type,
         .offset = offsetof (CarState, state) + offsetof (RocketSim::CarState, updateCounter),
         .flags  = 0,
@@ -123,14 +126,18 @@
         .offset = offsetof (CarState, state) + offsetof (RocketSim::CarState, demoRespawnTimer),
         .flags  = 0,
         .doc    = "Demo respawn timer"},
     {.name = nullptr, .type = 0, .offset = 0, .flags = 0, .doc = nullptr},
 };
 
 PyMethodDef CarState::Methods[] = {
+    {.ml_name     = "has_flip_or_jump",
+        .ml_meth  = (PyCFunction)&CarState::HasFlipOrJump,
+        .ml_flags = METH_NOARGS,
+        .ml_doc   = nullptr},
     {.ml_name = "__getstate__", .ml_meth = (PyCFunction)&CarState::Pickle, .ml_flags = METH_NOARGS, .ml_doc = nullptr},
     {.ml_name = "__setstate__", .ml_meth = (PyCFunction)&CarState::Unpickle, .ml_flags = METH_O, .ml_doc = nullptr},
     {.ml_name     = "__copy__",
         .ml_meth  = (PyCFunction)&CarState::Copy,
         .ml_flags = METH_NOARGS,
         .ml_doc   = R"(__copy__(self) -> RocketSim.CarState
 Shallow copy)"},
@@ -143,18 +150,19 @@
 };
 
 PyGetSetDef CarState::GetSet[] = {
     GETSET_ENTRY (CarState, pos, "Position"),
     GETSET_ENTRY (CarState, rot_mat, "Rotation matrix"),
     GETSET_ENTRY (CarState, vel, "Velocity"),
     GETSET_ENTRY (CarState, ang_vel, "Angular velocity"),
-    GETSET_ENTRY (CarState, last_rel_dodge_torque, "Last relative dodge torque"),
+    GETSET_ENTRY (CarState, flip_rel_torque, "Flip relative torque"),
     GETSET_ENTRY (CarState, last_controls, "Last controls"),
     GETSET_ENTRY (CarState, world_contact_normal, "World contact normal"),
     GETSET_ENTRY (CarState, ball_hit_info, "Ball hit info"),
+    GETSET_ENTRY (CarState, wheels_with_contact, "Wheels with contact"),
     {.name = nullptr, .get = nullptr, .set = nullptr, .doc = nullptr, .closure = nullptr},
 };
 
 PyType_Slot CarState::Slots[] = {
     {Py_tp_new, (void *)&CarState::New},
     {Py_tp_init, (void *)&CarState::Init},
     {Py_tp_dealloc, (void *)&CarState::Dealloc},
@@ -164,18 +172,19 @@
     {Py_tp_doc, (void *)R"(Car state
 __init__(self
 	pos: RocketSim.Vec = RocketSim.Vec(z = 17.0),
 	rot_mat: RocketSim.RotMat = RocketSim.RotMat(),
 	vel: RocketSim.Vec = RocketSim.Vec(),
 	ang_vel: RocketSim.Vec = RocketSim.Vec(),
 	is_on_ground: bool = True,
+	wheels_with_contact: Tuple[bool] = (false, false, false, false),
 	has_jumped: bool = False,
 	has_double_jumped: bool = False,
 	has_flipped: bool = False,
-	last_rel_dodge_torque: RocketSim.Vec = RocketSim.Vec(),
+	flip_rel_torque: RocketSim.Vec = RocketSim.Vec(),
 	jump_time: float = 0.0,
 	flip_time: float = 0.0,
 	is_flipping: bool = False,
 	is_jumping: bool = False,
 	air_time_since_jump: float = 0.0,
 	boost: float = 33.3,
 	time_spent_boosting: float = 0.0,
@@ -215,28 +224,27 @@
 
 bool CarState::InitFromCarState (CarState *const self_, RocketSim::CarState const &state_) noexcept
 {
 	auto pos                = Vec::NewFromVec (state_.pos);
 	auto rotMat             = RotMat::NewFromRotMat (state_.rotMat);
 	auto vel                = Vec::NewFromVec (state_.vel);
 	auto angVel             = Vec::NewFromVec (state_.angVel);
-	auto lastRelDodgeTorque = Vec::NewFromVec (state_.lastRelDodgeTorque);
+	auto flipRelTorque      = Vec::NewFromVec (state_.flipRelTorque);
 	auto lastControls       = CarControls::NewFromCarControls (state_.lastControls);
 	auto worldContactNormal = Vec::NewFromVec (state_.worldContact.contactNormal);
 	auto ballHitInfo        = BallHitInfo::NewFromBallHitInfo (state_.ballHitInfo);
 
-	if (!pos || !rotMat || !vel || !angVel || !lastRelDodgeTorque || !lastControls || !worldContactNormal ||
-	    !ballHitInfo)
+	if (!pos || !rotMat || !vel || !angVel || !flipRelTorque || !lastControls || !worldContactNormal || !ballHitInfo)
 		return false;
 
 	PyRef<Vec>::assign (self_->pos, pos.borrowObject ());
 	PyRef<RotMat>::assign (self_->rotMat, rotMat.borrowObject ());
 	PyRef<Vec>::assign (self_->vel, vel.borrowObject ());
 	PyRef<Vec>::assign (self_->angVel, angVel.borrowObject ());
-	PyRef<Vec>::assign (self_->lastRelDodgeTorque, lastRelDodgeTorque.borrowObject ());
+	PyRef<Vec>::assign (self_->flipRelTorque, flipRelTorque.borrowObject ());
 	PyRef<CarControls>::assign (self_->lastControls, lastControls.borrowObject ());
 	PyRef<Vec>::assign (self_->worldContactNormal, worldContactNormal.borrowObject ());
 	PyRef<BallHitInfo>::assign (self_->ballHitInfo, ballHitInfo.borrowObject ());
 
 	self_->state = state_;
 
 	return true;
@@ -246,15 +254,15 @@
 {
 	auto state = self_->state;
 
 	state.pos                        = Vec::ToVec (self_->pos);
 	state.rotMat                     = RotMat::ToRotMat (self_->rotMat);
 	state.vel                        = Vec::ToVec (self_->vel);
 	state.angVel                     = Vec::ToVec (self_->angVel);
-	state.lastRelDodgeTorque         = Vec::ToVec (self_->lastRelDodgeTorque);
+	state.flipRelTorque              = Vec::ToVec (self_->flipRelTorque);
 	state.lastControls               = CarControls::ToCarControls (self_->lastControls);
 	state.worldContact.contactNormal = Vec::ToVec (self_->worldContactNormal);
 	state.ballHitInfo                = BallHitInfo::ToBallHitInfo (self_->ballHitInfo);
 
 	return state;
 }
 
@@ -268,33 +276,34 @@
 
 	new (&self->state) RocketSim::CarState ();
 
 	self->pos                = nullptr;
 	self->rotMat             = nullptr;
 	self->vel                = nullptr;
 	self->angVel             = nullptr;
-	self->lastRelDodgeTorque = nullptr;
+	self->flipRelTorque      = nullptr;
 	self->lastControls       = nullptr;
 	self->worldContactNormal = nullptr;
 	self->ballHitInfo        = nullptr;
 
 	return self.giftObject ();
 }
 
 int CarState::Init (CarState *self_, PyObject *args_, PyObject *kwds_) noexcept
 {
 	static char posKwd[]                     = "pos";
 	static char rotMatKwd[]                  = "rot_mat";
 	static char velKwd[]                     = "vel";
 	static char angVelKwd[]                  = "ang_vel";
 	static char isOnGroundKwd[]              = "is_on_ground";
+	static char wheelsWithContactKwd[]       = "wheels_with_contact";
 	static char hasJumpedKwd[]               = "has_jumped";
 	static char hasDoubleJumpedKwd[]         = "has_double_jumped";
 	static char hasFlippedKwd[]              = "has_flipped";
-	static char lastRelDodgeTorqueKwd[]      = "last_rel_dodge_torque";
+	static char flipRelTorqueKwd[]           = "flip_rel_torque";
 	static char jumpTimeKwd[]                = "jump_time";
 	static char flipTimeKwd[]                = "flip_time";
 	static char isFlippingKwd[]              = "is_flipping";
 	static char isJumpingKwd[]               = "is_jumping";
 	static char airTimeSinceJumpKwd[]        = "air_time_since_jump";
 	static char boostKwd[]                   = "boost";
 	static char timeSpentBoostingKwd[]       = "time_spent_boosting";
@@ -314,18 +323,19 @@
 	static char updateCounterKwd[]           = "update_counter";
 
 	static char *dict[] = {posKwd,
 	    rotMatKwd,
 	    velKwd,
 	    angVelKwd,
 	    isOnGroundKwd,
+	    wheelsWithContactKwd,
 	    hasJumpedKwd,
 	    hasDoubleJumpedKwd,
 	    hasFlippedKwd,
-	    lastRelDodgeTorqueKwd,
+	    flipRelTorqueKwd,
 	    jumpTimeKwd,
 	    flipTimeKwd,
 	    isFlippingKwd,
 	    isJumpingKwd,
 	    airTimeSinceJumpKwd,
 	    boostKwd,
 	    timeSpentBoostingKwd,
@@ -347,15 +357,16 @@
 
 	RocketSim::CarState state{};
 
 	PyObject *pos                = nullptr; // borrowed references
 	PyObject *rotMat             = nullptr;
 	PyObject *vel                = nullptr;
 	PyObject *angVel             = nullptr;
-	PyObject *lastRelDodgeTorque = nullptr;
+	PyObject *wheelsWithContact  = nullptr;
+	PyObject *flipRelTorque      = nullptr;
 	PyObject *lastControls       = nullptr;
 	PyObject *worldContactNormal = nullptr;
 	PyObject *ballHitInfo        = nullptr;
 
 	int isOnGround      = state.isOnGround;
 	int hasJumped       = state.hasJumped;
 	int hasDoubleJumped = state.hasDoubleJumped;
@@ -367,30 +378,31 @@
 	int hasWorldContact = state.worldContact.hasContact;
 	int isDemoed        = state.isDemoed;
 
 	unsigned long carContactID       = state.carContact.otherCarID;
 	unsigned long long updateCounter = state.updateCounter;
 	if (!PyArg_ParseTupleAndKeywords (args_,
 	        kwds_,
-	        "|O!O!O!O!ppppO!ffppfffpffpfpO!kfpfO!O!K",
+	        "|O!O!O!O!pOpppO!ffppfffpffpfpO!kfpfO!O!K",
 	        dict,
 	        Vec::Type,
 	        &pos,
 	        RotMat::Type,
 	        &rotMat,
 	        Vec::Type,
 	        &vel,
 	        Vec::Type,
 	        &angVel,
 	        &isOnGround,
+	        &wheelsWithContact,
 	        &hasJumped,
 	        &hasDoubleJumped,
 	        &hasFlipped,
 	        Vec::Type,
-	        &lastRelDodgeTorque,
+	        &flipRelTorque,
 	        &state.jumpTime,
 	        &state.flipTime,
 	        &isFlipping,
 	        &isJumping,
 	        &state.airTimeSinceJump,
 	        &state.boost,
 	        &state.timeSpentBoosting,
@@ -421,16 +433,25 @@
 
 	if (vel)
 		state.vel = Vec::ToVec (PyCast<Vec> (vel));
 
 	if (angVel)
 		state.angVel = Vec::ToVec (PyCast<Vec> (angVel));
 
-	if (lastRelDodgeTorque)
-		state.lastRelDodgeTorque = Vec::ToVec (PyCast<Vec> (lastRelDodgeTorque));
+	if (wheelsWithContact)
+	{
+		std::array<bool, NUM_WHEELS> tmp;
+		if (!fromSequence (wheelsWithContact, std::span (tmp)))
+			return -1;
+
+		std::copy (std::begin (tmp), std::end (tmp), std::begin (state.wheelsWithContact));
+	}
+
+	if (flipRelTorque)
+		state.flipRelTorque = Vec::ToVec (PyCast<Vec> (flipRelTorque));
 
 	if (worldContactNormal)
 		state.worldContact.contactNormal = Vec::ToVec (PyCast<Vec> (worldContactNormal));
 
 	if (ballHitInfo)
 		state.ballHitInfo = BallHitInfo::ToBallHitInfo (PyCast<BallHitInfo> (ballHitInfo));
 
@@ -459,15 +480,15 @@
 
 void CarState::Dealloc (CarState *self_) noexcept
 {
 	Py_XDECREF (self_->pos);
 	Py_XDECREF (self_->rotMat);
 	Py_XDECREF (self_->vel);
 	Py_XDECREF (self_->angVel);
-	Py_XDECREF (self_->lastRelDodgeTorque);
+	Py_XDECREF (self_->flipRelTorque);
 	Py_XDECREF (self_->lastControls);
 	Py_XDECREF (self_->worldContactNormal);
 	Py_XDECREF (self_->ballHitInfo);
 
 	self_->state.~CarState ();
 
 	auto const tp_free = (freefunc)PyType_GetSlot (Type, Py_tp_free);
@@ -501,28 +522,34 @@
 	if (state.angVel != model.angVel && !DictSetValue (dict.borrow (), "ang_vel", PyNewRef (self_->angVel)))
 		return nullptr;
 
 	if (state.isOnGround != model.isOnGround &&
 	    !DictSetValue (dict.borrow (), "is_on_ground", PyBool_FromLong (state.isOnGround)))
 		return nullptr;
 
+	if (!std::equal (std::begin (state.wheelsWithContact),
+	        std::end (state.wheelsWithContact),
+	        std::begin (model.wheelsWithContact)) &&
+	    !DictSetValue (dict.borrow (), "wheels_with_contact", Getwheels_with_contact (self_, nullptr)))
+		return nullptr;
+
 	if (state.hasJumped != model.hasJumped &&
 	    !DictSetValue (dict.borrow (), "has_jumped", PyBool_FromLong (state.hasJumped)))
 		return nullptr;
 
 	if (state.hasDoubleJumped != model.hasDoubleJumped &&
 	    !DictSetValue (dict.borrow (), "has_double_jumped", PyBool_FromLong (state.hasDoubleJumped)))
 		return nullptr;
 
 	if (state.hasFlipped != model.hasFlipped &&
 	    !DictSetValue (dict.borrow (), "has_flipped", PyBool_FromLong (state.hasFlipped)))
 		return nullptr;
 
-	if (state.lastRelDodgeTorque != model.lastRelDodgeTorque &&
-	    !DictSetValue (dict.borrow (), "last_rel_dodge_torque", PyNewRef (self_->lastRelDodgeTorque)))
+	if (state.flipRelTorque != model.flipRelTorque &&
+	    !DictSetValue (dict.borrow (), "flip_rel_torque", PyNewRef (self_->flipRelTorque)))
 		return nullptr;
 
 	if (state.jumpTime != model.jumpTime &&
 	    !DictSetValue (dict.borrow (), "jump_time", PyFloat_FromDouble (state.jumpTime)))
 		return nullptr;
 
 	if (state.flipTime != model.flipTime &&
@@ -632,15 +659,15 @@
 	if (!state)
 		return nullptr;
 
 	PyRef<Vec>::assign (state->pos, reinterpret_cast<PyObject *> (self_->pos));
 	PyRef<RotMat>::assign (state->rotMat, reinterpret_cast<PyObject *> (self_->rotMat));
 	PyRef<Vec>::assign (state->vel, reinterpret_cast<PyObject *> (self_->vel));
 	PyRef<Vec>::assign (state->angVel, reinterpret_cast<PyObject *> (self_->angVel));
-	PyRef<Vec>::assign (state->lastRelDodgeTorque, reinterpret_cast<PyObject *> (self_->lastRelDodgeTorque));
+	PyRef<Vec>::assign (state->flipRelTorque, reinterpret_cast<PyObject *> (self_->flipRelTorque));
 	PyRef<CarControls>::assign (state->lastControls, reinterpret_cast<PyObject *> (self_->lastControls));
 	PyRef<Vec>::assign (state->worldContactNormal, reinterpret_cast<PyObject *> (self_->worldContactNormal));
 	PyRef<BallHitInfo>::assign (state->ballHitInfo, reinterpret_cast<PyObject *> (self_->ballHitInfo));
 
 	state->state = ToCarState (self_);
 
 	return state.giftObject ();
@@ -664,16 +691,16 @@
 	if (!state->vel)
 		return nullptr;
 
 	PyRef<Vec>::assign (state->angVel, PyDeepCopy (self_->angVel, memo_));
 	if (!state->angVel)
 		return nullptr;
 
-	PyRef<Vec>::assign (state->lastRelDodgeTorque, PyDeepCopy (self_->lastRelDodgeTorque, memo_));
-	if (!state->lastRelDodgeTorque)
+	PyRef<Vec>::assign (state->flipRelTorque, PyDeepCopy (self_->flipRelTorque, memo_));
+	if (!state->flipRelTorque)
 		return nullptr;
 
 	PyRef<CarControls>::assign (state->lastControls, PyDeepCopy (self_->lastControls, memo_));
 	if (!state->lastControls)
 		return nullptr;
 
 	PyRef<Vec>::assign (state->worldContactNormal, PyDeepCopy (self_->worldContactNormal, memo_));
@@ -685,24 +712,29 @@
 		return nullptr;
 
 	state->state = ToCarState (self_);
 
 	return state.giftObject ();
 }
 
+PyObject *CarState::HasFlipOrJump (CarState *self_) noexcept
+{
+	return PyBool_FromLong (self_->state.HasFlipOrJump ());
+}
+
 PyObject *CarState::Getpos (CarState *self_, void *) noexcept
 {
 	return PyRef<Vec>::incRef (self_->pos).giftObject ();
 }
 
 int CarState::Setpos (CarState *self_, PyObject *value_, void *) noexcept
 {
 	if (!value_)
 	{
-		PyErr_SetString (PyExc_TypeError, "can't delete 'pos' attribute of 'RocketSim.CarState' objects");
+		PyErr_SetString (PyExc_AttributeError, "can't delete 'pos' attribute of 'RocketSim.CarState' objects");
 		return -1;
 	}
 
 	if (!Py_IS_TYPE (value_, Vec::Type))
 	{
 		PyErr_SetString (PyExc_TypeError, "attribute value type must be RocketSim.Vec");
 		return -1;
@@ -718,15 +750,15 @@
 	return PyRef<RotMat>::incRef (self_->rotMat).giftObject ();
 }
 
 int CarState::Setrot_mat (CarState *self_, PyObject *value_, void *) noexcept
 {
 	if (!value_)
 	{
-		PyErr_SetString (PyExc_TypeError, "can't delete 'rot_mat' attribute of 'RocketSim.CarState' objects");
+		PyErr_SetString (PyExc_AttributeError, "can't delete 'rot_mat' attribute of 'RocketSim.CarState' objects");
 		return -1;
 	}
 
 	if (!Py_IS_TYPE (value_, RotMat::Type))
 	{
 		PyErr_SetString (PyExc_TypeError, "attribute value type must be RocketSim.RotMat");
 		return -1;
@@ -742,15 +774,15 @@
 	return PyRef<Vec>::incRef (self_->vel).giftObject ();
 }
 
 int CarState::Setvel (CarState *self_, PyObject *value_, void *) noexcept
 {
 	if (!value_)
 	{
-		PyErr_SetString (PyExc_TypeError, "can't delete 'vel' attribute of 'RocketSim.CarState' objects");
+		PyErr_SetString (PyExc_AttributeError, "can't delete 'vel' attribute of 'RocketSim.CarState' objects");
 		return -1;
 	}
 
 	if (!Py_IS_TYPE (value_, Vec::Type))
 	{
 		PyErr_SetString (PyExc_TypeError, "attribute value type must be RocketSim.Vec");
 		return -1;
@@ -766,64 +798,65 @@
 	return PyRef<Vec>::incRef (self_->angVel).giftObject ();
 }
 
 int CarState::Setang_vel (CarState *self_, PyObject *value_, void *) noexcept
 {
 	if (!value_)
 	{
-		PyErr_SetString (PyExc_TypeError, "can't delete 'ang_vel' attribute of 'RocketSim.CarState' objects");
+		PyErr_SetString (PyExc_AttributeError, "can't delete 'ang_vel' attribute of 'RocketSim.CarState' objects");
 		return -1;
 	}
 
 	if (!Py_IS_TYPE (value_, Vec::Type))
 	{
 		PyErr_SetString (PyExc_TypeError, "attribute value type must be RocketSim.Vec");
 		return -1;
 	}
 
 	PyRef<Vec>::assign (self_->angVel, value_);
 
 	return 0;
 }
 
-PyObject *CarState::Getlast_rel_dodge_torque (CarState *self_, void *) noexcept
+PyObject *CarState::Getflip_rel_torque (CarState *self_, void *) noexcept
 {
-	return PyRef<Vec>::incRef (self_->lastRelDodgeTorque).giftObject ();
+	return PyRef<Vec>::incRef (self_->flipRelTorque).giftObject ();
 }
 
-int CarState::Setlast_rel_dodge_torque (CarState *self_, PyObject *value_, void *) noexcept
+int CarState::Setflip_rel_torque (CarState *self_, PyObject *value_, void *) noexcept
 {
 	if (!value_)
 	{
 		PyErr_SetString (
-		    PyExc_TypeError, "can't delete 'last_rel_dodge_torque' attribute of 'RocketSim.CarState' objects");
+		    PyExc_AttributeError, "can't delete 'flip_rel_torque' attribute of 'RocketSim.CarState' objects");
 		return -1;
 	}
 
 	if (!Py_IS_TYPE (value_, Vec::Type))
 	{
 		PyErr_SetString (PyExc_TypeError, "attribute value type must be RocketSim.Vec");
 		return -1;
 	}
 
-	PyRef<Vec>::assign (self_->lastRelDodgeTorque, value_);
+	PyRef<Vec>::assign (self_->flipRelTorque, value_);
 
 	return 0;
 }
 
 PyObject *CarState::Getlast_controls (CarState *self_, void *) noexcept
 {
 	return PyRef<CarControls>::incRef (self_->lastControls).giftObject ();
 }
 
 int CarState::Setlast_controls (CarState *self_, PyObject *value_, void *) noexcept
 {
 	if (!value_)
 	{
-		PyErr_SetString (PyExc_TypeError, "can't delete 'last_controls' attribute of 'RocketSim.CarState' objects");
+		PyErr_SetString (
+		    PyExc_AttributeError, "can't delete 'last_controls' attribute of 'RocketSim.CarState' objects");
 		return -1;
 	}
 
 	if (!Py_IS_TYPE (value_, CarControls::Type))
 	{
 		PyErr_SetString (PyExc_TypeError, "attribute value type must be RocketSim.CarControls");
 		return -1;
@@ -840,15 +873,15 @@
 }
 
 int CarState::Setworld_contact_normal (CarState *self_, PyObject *value_, void *) noexcept
 {
 	if (!value_)
 	{
 		PyErr_SetString (
-		    PyExc_TypeError, "can't delete 'world_contact_normal' attribute of 'RocketSim.CarState' objects");
+		    PyExc_AttributeError, "can't delete 'world_contact_normal' attribute of 'RocketSim.CarState' objects");
 		return -1;
 	}
 
 	if (!Py_IS_TYPE (value_, Vec::Type))
 	{
 		PyErr_SetString (PyExc_TypeError, "attribute value type must be RocketSim.Vec");
 		return -1;
@@ -864,22 +897,56 @@
 	return PyRef<BallHitInfo>::incRef (self_->ballHitInfo).giftObject ();
 }
 
 int CarState::Setball_hit_info (CarState *self_, PyObject *value_, void *) noexcept
 {
 	if (!value_)
 	{
-		PyErr_SetString (PyExc_TypeError, "can't delete 'ball_hit_info' attribute of 'RocketSim.CarState' objects");
+		PyErr_SetString (
+		    PyExc_AttributeError, "can't delete 'ball_hit_info' attribute of 'RocketSim.CarState' objects");
 		return -1;
 	}
 
 	if (!Py_IS_TYPE (value_, BallHitInfo::Type))
 	{
 		PyErr_SetString (PyExc_TypeError, "attribute value type must be RocketSim.BallHitInfo");
 		return -1;
 	}
 
 	PyRef<BallHitInfo>::assign (self_->ballHitInfo, value_);
 
 	return 0;
 }
+
+PyObject *CarState::Getwheels_with_contact (CarState *self_, void *) noexcept
+{
+	auto obj = PyObjectRef::stealObject (PyTuple_New (NUM_WHEELS));
+	if (!obj)
+		return nullptr;
+
+	for (unsigned i = 0; i < NUM_WHEELS; ++i)
+	{
+		if (PyTuple_SetItem (obj.borrow (), i, PyBool_FromLong (self_->state.wheelsWithContact[i])) != 0)
+			return nullptr;
+	}
+
+	return obj.giftObject ();
+}
+
+int CarState::Setwheels_with_contact (CarState *self_, PyObject *value_, void *) noexcept
+{
+	if (!value_)
+	{
+		PyErr_SetString (
+		    PyExc_TypeError, "can't delete 'wheels_with_contact' attribute of 'RocketSim.CarState' objects");
+		return -1;
+	}
+
+	std::array<bool, NUM_WHEELS> tmp;
+	if (!fromSequence (value_, std::span (tmp)))
+		return -1;
+
+	std::copy (std::begin (tmp), std::end (tmp), std::begin (self_->state.wheelsWithContact));
+
+	return 0;
+}
 }
```

### Comparing `RocketSim-2.1.0a2/python-mtheall/Module.cpp` & `RocketSim-2.1.0a3/python-mtheall/Module.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/python-mtheall/Module.h` & `RocketSim-2.1.0a3/python-mtheall/Module.h`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #include "Sim/Arena/Arena.h"
 #include "Sim/BallPredTracker/BallPredTracker.h"
 #include "Sim/Car/Car.h"
 #include "Sim/GameEventTracker/GameEventTracker.h"
 
 #include <map>
 #include <memory>
+#include <span>
 #include <unordered_map>
 #include <vector>
 
 #ifndef Py_UNREACHABLE
 #ifndef NDEBUG
 #define Py_UNREACHABLE() Py_FatalError ("Unreachable C code path reached")
 #elif defined(_MSC_VER)
@@ -92,14 +93,41 @@
 {
 void InitInternal (char const *path_);
 
 bool DictSetValue (PyObject *dict_, char const *key_, PyObject *value_) noexcept;
 
 PyObject *PyDeepCopy (void *obj_, PyObject *memo_) noexcept;
 
+template <typename T, std::size_t Extent>
+bool fromSequence (PyObject *obj_, std::span<T, Extent> span_) noexcept
+{
+	if (!PySequence_Check (obj_))
+	{
+		PyErr_SetString (PyExc_TypeError, "attribute value type must be a sequence");
+		return false;
+	}
+
+	if (PySequence_Size (obj_) != span_.size ())
+	{
+		PyErr_Format (PyExc_RuntimeError, "sequence must contain %u elements", static_cast<unsigned> (span_.size ()));
+		return false;
+	}
+
+	for (unsigned i = 0; i < span_.size (); ++i)
+	{
+		auto const obj = PyObjectRef::steal (PySequence_GetItem (obj_, i));
+		if (!obj)
+			return false;
+
+		span_[i] = PyObject_IsTrue (obj.borrow ());
+	}
+
+	return true;
+}
+
 class GIL
 {
 public:
 	~GIL () noexcept
 	{
 		PyGILState_Release (m_state);
 	}
@@ -501,15 +529,15 @@
 
 	RocketSim::CarState state;
 
 	Vec *pos;
 	RotMat *rotMat;
 	Vec *vel;
 	Vec *angVel;
-	Vec *lastRelDodgeTorque;
+	Vec *flipRelTorque;
 	CarControls *lastControls;
 	Vec *worldContactNormal;
 	BallHitInfo *ballHitInfo;
 
 	static PyRef<CarState> NewFromCarState (RocketSim::CarState const &state_ = {}) noexcept;
 	static bool InitFromCarState (CarState *self_, RocketSim::CarState const &state_ = {}) noexcept;
 	static RocketSim::CarState ToCarState (CarState *self_) noexcept;
@@ -525,22 +553,25 @@
 	static int Init (CarState *self_, PyObject *args_, PyObject *kwds_) noexcept;
 	static void Dealloc (CarState *self_) noexcept;
 	static PyObject *Pickle (CarState *self_) noexcept;
 	static PyObject *Unpickle (CarState *self_, PyObject *dict_) noexcept;
 	static PyObject *Copy (CarState *self_) noexcept;
 	static PyObject *DeepCopy (CarState *self_, PyObject *memo_) noexcept;
 
+	static PyObject *HasFlipOrJump (CarState *self_) noexcept;
+
 	GETSET_DECLARE (CarState, pos)
 	GETSET_DECLARE (CarState, rot_mat)
 	GETSET_DECLARE (CarState, vel)
 	GETSET_DECLARE (CarState, ang_vel)
-	GETSET_DECLARE (CarState, last_rel_dodge_torque)
+	GETSET_DECLARE (CarState, flip_rel_torque)
 	GETSET_DECLARE (CarState, last_controls)
 	GETSET_DECLARE (CarState, world_contact_normal)
 	GETSET_DECLARE (CarState, ball_hit_info)
+	GETSET_DECLARE (CarState, wheels_with_contact)
 };
 
 struct Car
 {
 	PyObject_HEAD;
 
 	RocketSim::CarState demoState;
```

### Comparing `RocketSim-2.1.0a2/python-mtheall/MutatorConfig.cpp` & `RocketSim-2.1.0a3/python-mtheall/MutatorConfig.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -606,15 +606,15 @@
 	return PyRef<Vec>::incRef (self_->gravity).giftObject ();
 }
 
 int MutatorConfig::Setgravity (MutatorConfig *self_, PyObject *value_, void *) noexcept
 {
 	if (!value_)
 	{
-		PyErr_SetString (PyExc_TypeError, "can't delete 'gravity' attribute of 'RocketSim.MutatorConfig' objects");
+		PyErr_SetString (PyExc_AttributeError, "can't delete 'gravity' attribute of 'RocketSim.MutatorConfig' objects");
 		return -1;
 	}
 
 	if (!Py_IS_TYPE (value_, Vec::Type))
 	{
 		PyErr_SetString (PyExc_TypeError, "attribute value type must be RocketSim.Vec");
 		return -1;
```

### Comparing `RocketSim-2.1.0a2/python-mtheall/PyRef.h` & `RocketSim-2.1.0a3/python-mtheall/PyRef.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/python-mtheall/RotMat.cpp` & `RocketSim-2.1.0a3/python-mtheall/RotMat.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -298,15 +298,15 @@
 	return PyRef<Vec>::incRef (self_->forward).giftObject ();
 }
 
 int RotMat::Setforward (RotMat *self_, PyObject *value_, void *) noexcept
 {
 	if (!value_)
 	{
-		PyErr_SetString (PyExc_TypeError, "can't delete 'forward' attribute of 'RocketSim.RotMat' objects");
+		PyErr_SetString (PyExc_AttributeError, "can't delete 'forward' attribute of 'RocketSim.RotMat' objects");
 		return -1;
 	}
 
 	if (!Py_IS_TYPE (value_, Vec::Type))
 	{
 		PyErr_SetString (PyExc_TypeError, "attribute value type must be RocketSim.Vec");
 		return -1;
@@ -322,15 +322,15 @@
 	return PyRef<Vec>::incRef (self_->right).giftObject ();
 }
 
 int RotMat::Setright (RotMat *self_, PyObject *value_, void *) noexcept
 {
 	if (!value_)
 	{
-		PyErr_SetString (PyExc_TypeError, "can't delete 'right' attribute of 'RocketSim.RotMat' objects");
+		PyErr_SetString (PyExc_AttributeError, "can't delete 'right' attribute of 'RocketSim.RotMat' objects");
 		return -1;
 	}
 
 	if (!Py_IS_TYPE (value_, Vec::Type))
 	{
 		PyErr_SetString (PyExc_TypeError, "attribute value type must be RocketSim.Vec");
 		return -1;
@@ -346,15 +346,15 @@
 	return PyRef<Vec>::incRef (self_->up).giftObject ();
 }
 
 int RotMat::Setup (RotMat *self_, PyObject *value_, void *) noexcept
 {
 	if (!value_)
 	{
-		PyErr_SetString (PyExc_TypeError, "can't delete 'up' attribute of 'RocketSim.RotMat' objects");
+		PyErr_SetString (PyExc_AttributeError, "can't delete 'up' attribute of 'RocketSim.RotMat' objects");
 		return -1;
 	}
 
 	if (!Py_IS_TYPE (value_, Vec::Type))
 	{
 		PyErr_SetString (PyExc_TypeError, "attribute value type must be RocketSim.Vec");
 		return -1;
```

### Comparing `RocketSim-2.1.0a2/python-mtheall/Vec.cpp` & `RocketSim-2.1.0a3/python-mtheall/Vec.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/python-mtheall/WheelPairConfig.cpp` & `RocketSim-2.1.0a3/python-mtheall/WheelPairConfig.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -215,16 +215,16 @@
 	return PyRef<Vec>::incRef (self_->connectionPointOffset).giftObject ();
 }
 
 int WheelPairConfig::Setconnection_point_offset (WheelPairConfig *self_, PyObject *value_, void *) noexcept
 {
 	if (!value_)
 	{
-		PyErr_SetString (
-		    PyExc_TypeError, "can't delete 'connection_point_offset' attribute of 'RocketSim.WheelPairConfig' objects");
+		PyErr_SetString (PyExc_AttributeError,
+		    "can't delete 'connection_point_offset' attribute of 'RocketSim.WheelPairConfig' objects");
 		return -1;
 	}
 
 	if (!Py_IS_TYPE (value_, Vec::Type))
 	{
 		PyErr_SetString (PyExc_TypeError, "attribute value type must be RocketSim.Vec");
 		return -1;
```

### Comparing `RocketSim-2.1.0a2/python-mtheall/regression_test.py` & `RocketSim-2.1.0a3/python-mtheall/regression_test.py`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/python-mtheall/unit_test.py` & `RocketSim-2.1.0a3/python-mtheall/unit_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -721,18 +721,19 @@
     self.assertAlmostEqual(state_a.pos,                  state_b.pos, 3)
     self.assertEqual(state_a.rot_mat.forward,            state_b.rot_mat.forward)
     self.assertEqual(state_a.rot_mat.right,              state_b.rot_mat.right)
     self.assertEqual(state_a.rot_mat.up,                 state_b.rot_mat.up)
     self.assertAlmostEqual(state_a.vel,                  state_b.vel, 3)
     self.assertEqual(state_a.ang_vel,                    state_b.ang_vel)
     self.assertEqual(state_a.is_on_ground,               state_b.is_on_ground)
+    self.assertEqual(state_a.wheels_with_contact,        state_b.wheels_with_contact)
     self.assertEqual(state_a.has_jumped,                 state_b.has_jumped)
     self.assertEqual(state_a.has_double_jumped,          state_b.has_double_jumped)
     self.assertEqual(state_a.has_flipped,                state_b.has_flipped)
-    self.assertEqual(state_a.last_rel_dodge_torque,      state_b.last_rel_dodge_torque)
+    self.assertEqual(state_a.flip_rel_torque,            state_b.flip_rel_torque)
     self.assertEqual(state_a.jump_time,                  state_b.jump_time)
     self.assertEqual(state_a.flip_time,                  state_b.flip_time)
     self.assertEqual(state_a.is_jumping,                 state_b.is_jumping)
     self.assertEqual(state_a.air_time_since_jump,        state_b.air_time_since_jump)
     self.assertEqual(state_a.boost,                      state_b.boost)
     self.assertEqual(state_a.time_spent_boosting,        state_b.time_spent_boosting)
     self.assertEqual(state_a.is_supersonic,              state_b.is_supersonic)
@@ -757,18 +758,19 @@
   def test_pickle(self):
     state_a = rs.CarState(
       pos                        = random_vec(),
       rot_mat                    = random_mat(),
       vel                        = random_vec(),
       ang_vel                    = random_vec(),
       is_on_ground               = random_bool(),
+      wheels_with_contact        = (random_bool(), random_bool(), random_bool(), random_bool()),
       has_jumped                 = random_bool(),
       has_double_jumped          = random_bool(),
       has_flipped                = random_bool(),
-      last_rel_dodge_torque      = random_vec(),
+      flip_rel_torque            = random_vec(),
       jump_time                  = random_float(),
       flip_time                  = random_float(),
       is_flipping                = random_bool(),
       is_jumping                 = random_bool(),
       air_time_since_jump        = random_float(),
       boost                      = random_float(),
       time_spent_boosting        = random_float(),
@@ -811,18 +813,19 @@
   def test_copy(self):
     state_a = rs.CarState(
       pos                        = random_vec(),
       rot_mat                    = random_mat(),
       vel                        = random_vec(),
       ang_vel                    = random_vec(),
       is_on_ground               = random_bool(),
+      wheels_with_contact        = (random_bool(), random_bool(), random_bool(), random_bool()),
       has_jumped                 = random_bool(),
       has_double_jumped          = random_bool(),
       has_flipped                = random_bool(),
-      last_rel_dodge_torque      = random_vec(),
+      flip_rel_torque            = random_vec(),
       jump_time                  = random_float(),
       flip_time                  = random_float(),
       is_flipping                = random_bool(),
       is_jumping                 = random_bool(),
       air_time_since_jump        = random_float(),
       boost                      = random_float(),
       time_spent_boosting        = random_float(),
@@ -872,18 +875,19 @@
   def test_deep_copy(self):
     state_a = rs.CarState(
       pos                        = random_vec(),
       rot_mat                    = random_mat(),
       vel                        = random_vec(),
       ang_vel                    = random_vec(),
       is_on_ground               = random_bool(),
+      wheels_with_contact        = (random_bool(), random_bool(), random_bool(), random_bool()),
       has_jumped                 = random_bool(),
       has_double_jumped          = random_bool(),
       has_flipped                = random_bool(),
-      last_rel_dodge_torque      = random_vec(),
+      flip_rel_torque            = random_vec(),
       jump_time                  = random_float(),
       flip_time                  = random_float(),
       is_flipping                = random_bool(),
       is_jumping                 = random_bool(),
       air_time_since_jump        = random_float(),
       boost                      = random_float(),
       time_spent_boosting        = random_float(),
```

### Comparing `RocketSim-2.1.0a2/setup.py` & `RocketSim-2.1.0a3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,12 +84,13 @@
     ("NO_IMPORT_ARRAY", "1"),
     ("RS_DONT_LOG", "1")
   ]
 )
 
 setup(
   name = "RocketSim",
-  version = "2.1.0a2",
+  version = "2.1.0a3",
   description = "This is Rocket League!",
   cmdclass = {"build_ext": build_ext_ex},
-  ext_modules = [RocketSim]
+  ext_modules = [RocketSim],
+  install_requires = ["numpy"]
 )
```

### Comparing `RocketSim-2.1.0a2/src/BulletLink.h` & `RocketSim-2.1.0a3/src/BulletLink.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/src/CollisionMeshFile/CollisionMeshFile.cpp` & `RocketSim-2.1.0a3/src/CollisionMeshFile/CollisionMeshFile.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/src/CollisionMeshFile/CollisionMeshFile.h` & `RocketSim-2.1.0a3/src/CollisionMeshFile/CollisionMeshFile.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/src/DataStream/DataStreamIn.h` & `RocketSim-2.1.0a3/src/DataStream/DataStreamIn.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/src/DataStream/DataStreamOut.h` & `RocketSim-2.1.0a3/src/DataStream/DataStreamOut.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/src/Framework.h` & `RocketSim-2.1.0a3/src/Framework.h`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,19 @@
 #include <thread>
 #include <cstring>
 #include <array>
 
 #define _USE_MATH_DEFINES // for M_PI and similar
 #include <cmath>
 
+#ifdef _MSC_VER
+// Disable annoying truncation warnings on MSVC
+#pragma warning(disable: 4305 4244 4267)
+#endif
+
 typedef uint8_t byte;
 
 // Current millisecond time
 #define RS_CUR_MS() (std::chrono::duration_cast<std::chrono::milliseconds>(std::chrono::high_resolution_clock::now().time_since_epoch()).count())
 
 #define RS_MAX(a, b) ((a > b) ? a : b)
 #define RS_MIN(a, b) ((a < b) ? a : b)
@@ -74,16 +79,21 @@
 #endif
 #else
 #define RSAPI
 #endif
 
 #define RS_ALIGN_16 alignas(16)
 
+#ifndef RS_NO_NAMESPACE
 #define RS_NS_START namespace RocketSim {
 #define RS_NS_END }
+#else
+#define RS_NS_START
+#define RS_NS_END
+#endif
 
 template<typename ...Args>
 size_t __RS_GET_ARGUMENT_COUNT(Args ...) {
 	return sizeof...(Args);
 }
 #define RS_GET_ARGUMENT_COUNT __RS_GET_ARGUMENT_COUNT
```

### Comparing `RocketSim-2.1.0a2/src/Math/Math.cpp` & `RocketSim-2.1.0a3/src/Math/Math.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/src/Math/Math.h` & `RocketSim-2.1.0a3/src/Math/Math.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/src/Math/MathTypes/MathTypes.cpp` & `RocketSim-2.1.0a3/src/Math/MathTypes/MathTypes.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/src/Math/MathTypes/MathTypes.h` & `RocketSim-2.1.0a3/src/Math/MathTypes/MathTypes.h`

 * *Files 3% similar despite different names*

```diff
@@ -17,27 +17,45 @@
 		*(btVector3*)this = bulletVec;
 	}
 
 	bool IsZero() const {
 		return (x == 0 && y == 0 && z == 0 && _w == 0);
 	}
 
+	// Makes a copy with zeroed z
+	Vec To2D() const {
+		return Vec(x, y, 0);
+	}
+
 	float LengthSq() const {
 		return (x * x + y * y + z * z + _w * _w);
 	}
 
 	float Length() const {
 		float lengthSq = LengthSq();
 		if (lengthSq > 0) {
 			return sqrtf(lengthSq);
 		} else {
 			return 0;
 		}
 	}
 
+	float LengthSq2D() const {
+		return (x * x + y * y);
+	}
+
+	float Length2D() const {
+		float lengthSq2D = LengthSq2D();
+		if (lengthSq2D > 0) {
+			return sqrtf(lengthSq2D);
+		} else {
+			return 0;
+		}
+	}
+
 	float Dot(const Vec& other) const {
 		return (x * other.x + y * other.y + z * other.z + _w * other._w);
 	}
 
 	Vec Cross(const Vec& other) const {
 		return Vec(
 			(y * other.z) - (z * other.y),
@@ -227,17 +245,17 @@
 			vec.Dot(up)
 		);
 	}
 
 	RotMat Dot(const RotMat& other) const {
 		RotMat result;
 
-		for (size_t i = 0; i < 3; i++)
-			for (size_t j = 0; j < 3; j++)
-				for (size_t k = 0; k < 3; k++)
+		for (int i = 0; i < 3; i++)
+			for (int j = 0; j < 3; j++)
+				for (int k = 0; k < 3; k++)
 					result[i][j] += (*this)[i][j] * other[k][j];
 
 		return result;
 	}
 
 	RotMat Transpose() const {
 		RotMat result;
```

### Comparing `RocketSim-2.1.0a2/src/RLConst.h` & `RocketSim-2.1.0a3/src/RLConst.h`

 * *Files 0% similar despite different names*

```diff
@@ -99,21 +99,21 @@
 		FLIP_TORQUE_Y = 224.f, // Forward/backward
 		FLIP_FORWARD_IMPULSE_MAX_SPEED_SCALE = 1.f,
 		FLIP_SIDE_IMPULSE_MAX_SPEED_SCALE = 1.9f,
 		FLIP_BACKWARD_IMPULSE_MAX_SPEED_SCALE = 2.5f,
 		FLIP_BACKWARD_IMPULSE_SCALE_X = 16.f / 15.f,
 
 		BALL_COLLISION_RADIUS_SOCCAR = 91.25f,
-		BALL_COLLISION_RADIUS_HOOPS = 96.38307f,
-		BALL_COLLISION_RADIUS_DROPSHOT = 100.2565,
+		BALL_COLLISION_RADIUS_HOOPS = 96.3831f,
+		BALL_COLLISION_RADIUS_DROPSHOT = 100.2565f,
 
 		SOCCAR_GOAL_SCORE_BASE_THRESHOLD_Y = 5124.25f,
 		HOOPS_GOAL_SCORE_THRESHOLD_Z = 270.f,
 
-		CAR_TORQUE_SCALE = 0.09587,
+		CAR_TORQUE_SCALE = 0.09587f,
 
 		CAR_AUTOFLIP_IMPULSE = 200,
 		CAR_AUTOFLIP_TORQUE = 50,
 		CAR_AUTOFLIP_TIME = 0.4f,
 		CAR_AUTOFLIP_NORMZ_THRESH = M_SQRT1_2,
 		CAR_AUTOFLIP_ROLL_THRESH = 2.8f,
 
@@ -270,15 +270,15 @@
 
 		constexpr Vec LOCS_BIG_HOOPS[LOCS_AMOUNT_BIG] = {
 			{-2176,		 2944, 72 },
 			{ 2176,		-2944, 72 },
 			{-2176,		-2944, 72 },
 			{-2432,			0, 72 },
 			{ 2432,			0, 72 },
-			{ 2175.99,	 2944, 72 }
+			{ 2175.99f,	 2944, 72 }
 		};
 	}
 
 	constexpr int
 		CAR_SPAWN_LOCATION_AMOUNT = 5,
 		CAR_RESPAWN_LOCATION_AMOUNT = 4;
```

### Comparing `RocketSim-2.1.0a2/src/RocketSim.cpp` & `RocketSim-2.1.0a3/src/RocketSim.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -43,19 +43,19 @@
 };
 
 static RocketSimStage stage = RocketSimStage::UNINITIALIZED;
 RocketSimStage RocketSim::GetStage() {
 	return stage;
 }
 
-std::vector<btBvhTriangleMeshShape*>& RocketSim::GetArenaCollisionShapes(RocketSim::GameMode gameMode) {
+std::vector<btBvhTriangleMeshShape*>& RocketSim::GetArenaCollisionShapes(GameMode gameMode) {
 	static std::vector<btBvhTriangleMeshShape*> arenaCollisionMeshes;
 	static std::vector<btBvhTriangleMeshShape*> arenaCollisionMeshes_hoops;
 
-	return (gameMode == RocketSim::GameMode::HOOPS ? arenaCollisionMeshes_hoops : arenaCollisionMeshes);
+	return (gameMode == GameMode::HOOPS ? arenaCollisionMeshes_hoops : arenaCollisionMeshes);
 }
 
 #ifndef RS_NO_SUSPCOLGRID
 static SuspensionCollisionGrid
 	suspColGrids_soccar[] = { {GameMode::SOCCAR, true}, {GameMode::SOCCAR, false} },
 	suspColGrids_hoops[] = { {GameMode::HOOPS, true}, {GameMode::HOOPS, false} };
 	SuspensionCollisionGrid& RocketSim::GetDefaultSuspColGrid(GameMode gameMode, bool isLight) {
```

### Comparing `RocketSim-2.1.0a2/src/RocketSim.h` & `RocketSim-2.1.0a3/src/RocketSim.h`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 #include "Math/Math.h"
 
 // AVAILABLE DEFS FOR ROCKETSIM:
 //	RS_MAX_SPEED: Define this to remove certain sanity checks for faster speed
 //	RS_DONT_LOG: Define this to disable all logging output
 //	RS_NO_SUSPCOLGRID: Disable the suspension-collision grid optimization
+//	RS_NO_NAMESPACE: Disable the RocketSim namespace encapsulating all RocketSim classes/structs
 
 class btBvhTriangleMeshShape;
 
 namespace RocketSim {
 	enum class RocketSimStage : byte {
 		UNINITIALIZED,
 		INITIALIZING,
```

### Comparing `RocketSim-2.1.0a2/src/Sim/Arena/Arena.cpp` & `RocketSim-2.1.0a3/src/Sim/Arena/Arena.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -231,14 +231,17 @@
 	const btCollisionObjectWrapper* objA, int partID_A, int indexA,
 	const btCollisionObjectWrapper* objB, int partID_B, int indexB) {
 
 	auto
 		bodyA = objA->m_collisionObject,
 		bodyB = objB->m_collisionObject;
 
+	if (!objA->m_collisionObject->hasContactResponse() || !objB->m_collisionObject->hasContactResponse())
+		return true;
+
 	bool shouldSwap = false;
 	if ((bodyA->getUserIndex() != -1) && (bodyB->getUserIndex() != -1)) {
 		// If both bodies have a user index, the lower user index should be A
 		shouldSwap = bodyA->getUserIndex() > bodyB->getUserIndex();
 	} else {
 		// If only one body has a user index, make sure that body is A
 		shouldSwap = (bodyB->getUserIndex() != -1);
@@ -477,15 +480,15 @@
 			&_bulletWorldParams.collisionConfig
 		);
 
 		_bulletWorld.setGravity(_mutatorConfig.gravity * UU_TO_BT);
 
 		// Adjust solver configuration to be closer to older Bullet (Rocket League's Bullet is from somewhere between 2013 and 2015)
 		auto& solverInfo = _bulletWorld.getSolverInfo();
-		solverInfo.m_splitImpulsePenetrationThreshold = 1.0e30;
+		solverInfo.m_splitImpulsePenetrationThreshold = 1.0e30f;
 		solverInfo.m_erp2 = 0.8f;
 	}
 
 	bool loadArenaStuff = gameMode != GameMode::THE_VOID;
 
 	if (loadArenaStuff) {
 		_SetupArenaCollisionShapes();
@@ -593,15 +596,15 @@
 	in.ReadMultiple(gameMode, tickTime, tickCount, lastCarID, memWeightMode);
 
 	Arena* newArena = new Arena(gameMode, memWeightMode, 1.f / tickTime);
 	newArena->tickCount = tickCount;
 	
 	{ // Deserialize cars
 		uint32_t carAmount = in.Read<uint32_t>();
-		for (int i = 0; i < carAmount; i++) {
+		for (uint32_t i = 0; i < carAmount; i++) {
 			Team team;
 			uint32_t id;
 			in.Read(team);
 			in.Read(id);
 
 #ifndef RS_MAX_SPEED
 			if (newArena->_carIDMap.count(id))
```

### Comparing `RocketSim-2.1.0a2/src/Sim/Arena/Arena.h` & `RocketSim-2.1.0a3/src/Sim/Arena/Arena.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/src/Sim/Ball/Ball.cpp` & `RocketSim-2.1.0a3/src/Sim/Ball/Ball.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/src/Sim/Ball/Ball.h` & `RocketSim-2.1.0a3/src/Sim/Ball/Ball.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,46 @@
 #pragma once
-#include "../../BaseInc.h"
+#include "../PhysState/PhysState.h"
 
 #include "../../RLConst.h"
 #include "../../DataStream/DataStreamIn.h"
 #include "../../DataStream/DataStreamOut.h"
 
 #include "../MutatorConfig/MutatorConfig.h"
 
 #include "../../../libsrc/bullet3-3.24/BulletDynamics/Dynamics/btRigidBody.h"
 #include "../../../libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btSphereShape.h"
 
 class btDynamicsWorld;
 
 RS_NS_START
 
-struct BallState {
+struct BallState : public PhysState {
 	// Incremented every update, reset when SetState() is called
 	// Used for telling if a stateset occured
 	// Not serialized
 	uint64_t updateCounter = 0;
 
-	// Position in world space
-	Vec pos = { 0, 0, RLConst::BALL_REST_Z };
-
-	RotMat rotMat = RotMat::GetIdentity();
-
-	// Linear velocity
-	Vec vel = { 0, 0, 0 };
-	 
-	// Angular velocity (axis-angle)
-	Vec angVel = { 0, 0, 0 };
-
 	struct HeatseekerInfo {
 		// Which net the ball should seek towards
 		// When 0, no net
 		float yTargetDir = 0;
 
 		float curTargetSpeed = RLConst::Heatseeker::INITIAL_TARGET_SPEED;
 		float timeSinceHit = 0;
 	};
 
 	HeatseekerInfo hsInfo;
 
 	std::uint32_t lastHitCarID = 0;
 
+	BallState() : PhysState() {
+		pos.z = RLConst::BALL_REST_Z;
+	}
+
 	bool Matches(const BallState& other, float marginPos = 0.8, float marginVel = 0.4, float marginAngVel = 0.02) const;
 
 	void Serialize(DataStreamOut& out);
 	void Deserialize(DataStreamIn& in);
 };
 
 #define BALLSTATE_SERIALIZATION_FIELDS \
@@ -83,15 +76,15 @@
 
 	// Returns radius in Unreal Engine units (uu)
 	float GetRadius() const {
 		return GetRadiusBullet() * BT_TO_UU;
 	}
 
 	void _PreTickUpdate(GameMode gameMode, float tickTime);
-	void _OnHit(GameMode gameMode, struct Car* car);
+	void _OnHit(GameMode gameMode, class Car* car);
 	void _OnWorldCollision(GameMode gameMode, Vec normal, float tickTime);
 		
 	Ball(const Ball& other) = delete;
 	Ball& operator=(const Ball& other) = delete;
 
 	~Ball() {
 		delete _collisionShape;
```

### Comparing `RocketSim-2.1.0a2/src/Sim/BallHitInfo/BallHitInfo.h` & `RocketSim-2.1.0a3/src/Sim/BallHitInfo/BallHitInfo.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/src/Sim/BallPredTracker/BallPredTracker.cpp` & `RocketSim-2.1.0a3/src/Sim/BallPredTracker/BallPredTracker.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/src/Sim/BallPredTracker/BallPredTracker.h` & `RocketSim-2.1.0a3/src/Sim/BallPredTracker/BallPredTracker.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/src/Sim/BoostPad/BoostPad.cpp` & `RocketSim-2.1.0a3/src/Sim/BoostPad/BoostPad.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/src/Sim/BoostPad/BoostPad.h` & `RocketSim-2.1.0a3/src/Sim/BoostPad/BoostPad.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/src/Sim/BoostPad/BoostPadGrid/BoostPadGrid.cpp` & `RocketSim-2.1.0a3/src/Sim/BoostPad/BoostPadGrid/BoostPadGrid.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/src/Sim/BoostPad/BoostPadGrid/BoostPadGrid.h` & `RocketSim-2.1.0a3/src/Sim/BoostPad/BoostPadGrid/BoostPadGrid.h`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 		EXTENT_X = 4096.f,
 		EXTENT_Y = 5120.f,
 		EXTENT_Z = RLConst::BoostPads::CYL_HEIGHT + 250.f;
 
 	constexpr static int
 		CELLS_X = 8,
 		CELLS_Y = 10,
-		CELL_SIZE_X = EXTENT_X / (CELLS_X / 2),
-		CELL_SIZE_Y = EXTENT_Y / (CELLS_Y / 2),
+		CELL_SIZE_X = (int)(EXTENT_X / (CELLS_X / 2)),
+		CELL_SIZE_Y = (int)(EXTENT_Y / (CELLS_Y / 2)),
 		CELL_AMOUNT = CELLS_X * CELLS_Y;
 
 	BoostPad* pads[CELLS_X][CELLS_Y] = {};
 
 	BoostPadGrid() = default;
 
 	void CheckCollision(Car* car);
```

### Comparing `RocketSim-2.1.0a2/src/Sim/Car/Car.cpp` & `RocketSim-2.1.0a3/src/Sim/Car/Car.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -129,17 +129,21 @@
 void Car::_PostTickUpdate(GameMode gameMode, float tickTime, const MutatorConfig& mutatorConfig) {
 
 	if (_internalState.isDemoed)
 		return;
 
 	_internalState.rotMat = _rigidBody.m_worldTransform.m_basis;
 
+	// Update wheelsWithContact
 	int numWheelsInContact = 0;
-	for (int i = 0; i < 4; i++)
-		numWheelsInContact += _bulletVehicle.m_wheelInfo[i].m_raycastInfo.m_isInContact;
+	for (int i = 0; i < 4; i++) {
+		bool inContact = _bulletVehicle.m_wheelInfo[i].m_raycastInfo.m_isInContact;
+		_internalState.wheelsWithContact[i] = inContact;
+		numWheelsInContact += inContact;
+	}
 
 	{ // Update isOnGround
 		_internalState.isOnGround = numWheelsInContact >= 3;
 	}
 
 	{ // Update supersonic
 		float speedSquared = (_rigidBody.m_linearVelocity * BT_TO_UU).length2();
@@ -285,14 +289,20 @@
 			}
 		}
 	}
 
 	_internalState.boost = mutatorConfig.carSpawnBoostAmount;
 }
 
+bool CarState::HasFlipOrJump() const {
+	return 
+		isOnGround || 
+		(!hasFlipped && !hasDoubleJumped && airTimeSinceJump < RLConst::DOUBLEJUMP_MAX_DELAY);
+}
+
 void CarState::Serialize(DataStreamOut& out) const {
 	ballHitInfo.Serialize(out);
 
 	out.WriteMultiple(
 		CARSTATE_SERIALIZATION_FIELDS
 	);
 }
@@ -345,15 +355,15 @@
 		realThrottle = 1;
 
 	{ // Update throttle/brake forces
 		float driveSpeedScale = DRIVE_SPEED_TORQUE_FACTOR_CURVE.GetOutput(absForwardSpeed_UU);
 
 		float engineThrottle = realThrottle;
 
-		if (controls.handbrake > 0) {
+		if (controls.handbrake) {
 			// Real throttle is unchanged from the input throttle when powersliding
 		} else {
 			float absThrottle = abs(realThrottle);
 
 			if (absThrottle >= THROTTLE_DEADZONE) {
 				if (absForwardSpeed_UU > STOPPING_FORWARD_VEL && RS_SGN(realThrottle) != RS_SGN(forwardSpeed_UU)) {
 					// Full brake is applied if we are trying to drive in the opposite direction
@@ -552,17 +562,17 @@
 
 	bool doAirControl = false;
 	if (_internalState.isFlipping)
 		_internalState.isFlipping = _internalState.hasFlipped && _internalState.flipTime < FLIP_TORQUE_TIME;
 
 	if (_internalState.isFlipping) {
 
-		btVector3 relDodgeTorque = _internalState.lastRelDodgeTorque;
+		btVector3 relDodgeTorque = _internalState.flipRelTorque;
 
-		if (!_internalState.lastRelDodgeTorque.IsZero()) {
+		if (!_internalState.flipRelTorque.IsZero()) {
 			// Flip cancel check
 			float pitchScale = 1;
 			if (relDodgeTorque.y() != 0 && controls.pitch != 0) {
 				if (RS_SGN(relDodgeTorque.y()) == RS_SGN(controls.pitch)) {
 
 #ifndef RS_MAX_SPEED
 					pitchScale = 1 - RS_MIN(abs(controls.pitch), 1); // Sanity clamp
@@ -675,15 +685,15 @@
 
 						if (abs(controls.yaw + controls.roll) < 0.1f && abs(controls.pitch) < 0.1f) {
 							dodgeDir = { 0, 0, 0 };
 						} else {
 							dodgeDir = dodgeDir.safeNormalized();
 						}
 
-						_internalState.lastRelDodgeTorque = btVector3(-dodgeDir.y(), dodgeDir.x(), 0);
+						_internalState.flipRelTorque = btVector3(-dodgeDir.y(), dodgeDir.x(), 0);
 
 						if (abs(dodgeDir.x()) < 0.1f) dodgeDir.x() = 0;
 						if (abs(dodgeDir.y()) < 0.1f) dodgeDir.y() = 0;
 
 						if (!dodgeDir.fuzzyZero()) {
 							bool shouldDodgeBackwards;
```

### Comparing `RocketSim-2.1.0a2/src/Sim/Car/Car.h` & `RocketSim-2.1.0a3/src/Sim/Car/Car.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 #pragma once
+#include "../PhysState/PhysState.h"
 #include "CarConfig/CarConfig.h"
 #include "../btVehicleRL/btVehicleRL.h"
 #include "../CarControls.h"
 #include "../BallHitInfo/BallHitInfo.h"
 #include "../MutatorConfig/MutatorConfig.h"
 
 #include "../../../libsrc/bullet3-3.24/BulletDynamics/Dynamics/btRigidBody.h"
 #include "../../../libsrc/bullet3-3.24/BulletDynamics/Vehicle/btDefaultVehicleRaycaster.h"
 #include "../../../libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btBoxShape.h"
 #include "../../../libsrc/bullet3-3.24/BulletCollision/CollisionShapes/btCompoundShape.h"
 #include "../../../src/Sim/btVehicleRL/btVehicleRL.h"
 
 RS_NS_START
 
-struct CarState {
+struct CarState : public PhysState {
 
 	// Incremented every update, reset when SetState() is called
 	// Used for telling if a stateset occured
 	// Not serialized
 	uint64_t updateCounter = 0;
 
-	// Position in world space (UU)
-	Vec pos = { 0, 0, 17 };
-	
-	RotMat rotMat = RotMat::GetIdentity();
-
-	// Linear velocity
-	Vec vel = { 0, 0, 0 };
+	bool isOnGround = true;
 
-	// Angular velocity (rad/s)
-	Vec angVel = { 0, 0, 0 };
+	// Whether each of the 4 wheels have contact
+	// First two are front
+	bool wheelsWithContact[4] = {}; 
 
-	bool isOnGround = true;
 	bool hasJumped = false, hasDoubleJumped = false, hasFlipped = false;
-	Vec lastRelDodgeTorque = { 0, 0, 0 };
+	Vec flipRelTorque = { 0, 0, 0 };
 
 	// Active during the duration of a jump or flip
 	float jumpTime = 0, flipTime = 0;
 
 	// True during a flip (not a jump, and not after a flip)
 	bool isFlipping = false;
 
@@ -80,21 +75,28 @@
 	float demoRespawnTimer = 0;
 
 	BallHitInfo ballHitInfo = BallHitInfo();
 
 	// Controls from last tick, set to this->controls after simulation
 	CarControls lastControls = CarControls();
 
+	CarState() : PhysState() {
+		pos.z = RLConst::CAR_SPAWN_REST_Z;
+	}
+
+	// Returns true if the car is currently able to jump, double-jump, or start a flip
+	bool HasFlipOrJump() const;
+
 	void Serialize(DataStreamOut& out) const;
 	void Deserialize(DataStreamIn& in);
 };
 
 #define CARSTATE_SERIALIZATION_FIELDS \
 pos, rotMat, vel, angVel, isOnGround, hasJumped, hasDoubleJumped, hasFlipped, \
-lastRelDodgeTorque, jumpTime, isFlipping, flipTime, isJumping, airTimeSinceJump, \
+flipRelTorque, jumpTime, isFlipping, flipTime, isJumping, airTimeSinceJump, \
 boost, timeSpentBoosting, supersonicTime, handbrakeVal, isAutoFlipping, \
 autoFlipTimer, autoFlipTorqueScale, isDemoed, demoRespawnTimer, lastControls, \
 worldContact.hasContact, worldContact.contactNormal, \
 carContact.otherCarID, carContact.cooldownTimer
 
 enum class Team : byte {
 	BLUE = 0,
```

### Comparing `RocketSim-2.1.0a2/src/Sim/Car/CarConfig/CarConfig.cpp` & `RocketSim-2.1.0a3/src/Sim/Car/CarConfig/CarConfig.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 	{ -35.75f, 35.00f, 11.75f	},
 	{ -34.00f, 29.50f, 20.755f	},
 	{ -33.75f, 29.50f, 21.505f	}
 };
 
 // Using a macro here for convenience
 #define MAKE_CAR_CONFIG(name, index)                                                          \
-	const CarConfig CAR_CONFIG_##name = {                                                     \
+	const CarConfig CAR_CONFIG_##name = {                                          \
 		HITBOX_SIZES[index],                                                                  \
 		HITBOX_OFFSETS[index],                                                                \
 		{ FRONT_WHEEL_RADS[index], FRONT_WHEEL_SUS_REST[index], FRONT_WHEELS_OFFSET[index] }, \
 		{ BACK_WHEEL_RADS[index], BACK_WHEEL_SUS_REST[index], BACK_WHEELS_OFFSET[index] },    \
 	}
 
 MAKE_CAR_CONFIG(OCTANE, 0);
```

### Comparing `RocketSim-2.1.0a2/src/Sim/Car/CarConfig/CarConfig.h` & `RocketSim-2.1.0a3/src/Sim/Car/CarConfig/CarConfig.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/src/Sim/CarControls.h` & `RocketSim-2.1.0a3/src/Sim/CarControls.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/src/Sim/GameEventTracker/GameEventTracker.cpp` & `RocketSim-2.1.0a3/src/Sim/GameEventTracker/GameEventTracker.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -56,26 +56,27 @@
 
 		uint64_t deltaTicks = ballUpdateCount - _lastBallUpdateCount;
 
 		// Time since last update
 		float deltaTime = deltaTicks * arena->tickTime;
 
 		// Goal event
-		if (scored && _goalCallback.func && !_ballScoredLast) {
+		if (scored && !_ballScoredLast) {
 			Car* shooter;
 			Car* passer;
 			if (GetShooterPasser(
 				arena,
 				RS_TEAM_FROM_Y(-arena->ball->_rigidBody.m_worldTransform.m_origin.y()),
 				shooter, true, passer,
 				config.goalMaxTouchTime * tickrate,
 				config.passMaxTouchTime * tickrate
 			)) {
 
-				_goalCallback.func(arena, shooter, passer, _goalCallback.userInfo);
+				if (_goalCallback.func)
+					_goalCallback.func(arena, shooter, passer, _goalCallback.userInfo);
 			}
 		} else {
 			if (!_ballShot) { // Ball is not currently shot
 
 				if (_shotCooldown > 0) {
 					_shotCooldown = RS_MAX(_shotCooldown - deltaTime, 0);
 					// Can't make a shot yet
@@ -102,15 +103,16 @@
 								uint64_t ticksSinceHit = arena->tickCount - shooter->_internalState.ballHitInfo.tickCountWhenHit;
 								if (ticksSinceHit >= shotMinTouchDelayTicks) {
 
 									// This is officially now a shot!
 									_ballShot = true;
 									_ballShotGoalTeam = goalTeam;
 									_shotCooldown = config.shotEventCooldown;
-									_shotCallback.func(arena, shooter, passer, _shotCallback.userInfo);
+									if (_shotCallback.func)
+										_shotCallback.func(arena, shooter, passer, _shotCallback.userInfo);
 								}
 							}
 						}
 					}
 				}
 			} else {
 				// Ball is currently shot
@@ -128,15 +130,16 @@
 						saver, false, _unused,
 						deltaTicks,
 						0
 					)) {
 
 						// A car from the team the ball has just hit the ball
 						// Since it's no longer scoring, this was a save
-						_saveCallback.func(arena, saver, _saveCallback.userInfo);
+						if (_saveCallback.func)
+							_saveCallback.func(arena, saver, _saveCallback.userInfo);
 					} else {
 						// It just stopped going in (probably missed)
 					}
 					
 					_ballShot = false;
 				}
 			}
```

### Comparing `RocketSim-2.1.0a2/src/Sim/GameEventTracker/GameEventTracker.h` & `RocketSim-2.1.0a3/src/Sim/GameEventTracker/GameEventTracker.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/src/Sim/MutatorConfig/MutatorConfig.cpp` & `RocketSim-2.1.0a3/src/Sim/MutatorConfig/MutatorConfig.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/src/Sim/MutatorConfig/MutatorConfig.h` & `RocketSim-2.1.0a3/src/Sim/MutatorConfig/MutatorConfig.h`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/src/Sim/SuspensionCollisionGrid/SuspensionCollisionGrid.cpp` & `RocketSim-2.1.0a3/src/Sim/SuspensionCollisionGrid/SuspensionCollisionGrid.cpp`

 * *Files identical despite different names*

### Comparing `RocketSim-2.1.0a2/src/Sim/SuspensionCollisionGrid/SuspensionCollisionGrid.h` & `RocketSim-2.1.0a3/src/Sim/SuspensionCollisionGrid/SuspensionCollisionGrid.h`

 * *Files 2% similar despite different names*

```diff
@@ -77,17 +77,17 @@
 			CELL_SIZE_Y[LIGHT] * (yIndex - (CELL_AMOUNT_Y[LIGHT] / 2)),
 			CELL_SIZE_Z[LIGHT] * zIndex
 		);
 	}
 
 	template <bool LIGHT>
 	void GetCellIndicesFromPos(Vec pos, int& i, int& j, int& k) const {
-		i = RS_CLAMP(pos.x / CELL_SIZE_X[LIGHT] + (CELL_AMOUNT_X[LIGHT] / 2), 0, CELL_AMOUNT_X[LIGHT] - 1),
-		j = RS_CLAMP(pos.y / CELL_SIZE_Y[LIGHT] + (CELL_AMOUNT_Y[LIGHT] / 2), 0, CELL_AMOUNT_Y[LIGHT] - 1),
-		k = RS_CLAMP(pos.z / CELL_SIZE_Z[LIGHT], 0, CELL_AMOUNT_Z[LIGHT] - 1);
+		i = (int)RS_CLAMP(pos.x / CELL_SIZE_X[LIGHT] + (CELL_AMOUNT_X[LIGHT] / 2), 0, CELL_AMOUNT_X[LIGHT] - 1),
+		j = (int)RS_CLAMP(pos.y / CELL_SIZE_Y[LIGHT] + (CELL_AMOUNT_Y[LIGHT] / 2), 0, CELL_AMOUNT_Y[LIGHT] - 1),
+		k = (int)RS_CLAMP(pos.z / CELL_SIZE_Z[LIGHT], 0, CELL_AMOUNT_Z[LIGHT] - 1);
 	}
 
 	template <bool LIGHT>
 	Cell& GetCellFromPos(Vec pos) {
 		int i, j, k;
 		GetCellIndicesFromPos<LIGHT>(pos, i, j, k);
 		return Get<LIGHT>(i, j, k);
```

### Comparing `RocketSim-2.1.0a2/src/Sim/btVehicleRL/btVehicleRL.cpp` & `RocketSim-2.1.0a3/src/Sim/btVehicleRL/btVehicleRL.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 
 const btTransform& btVehicleRL::getWheelTransformWS(int wheelIndex) const {
 	btAssert(wheelIndex < getNumWheels());
 	const btWheelInfoRL& wheel = m_wheelInfo[wheelIndex];
 	return wheel.m_worldTransform;
 }
 
+// See: I20 or I21
 void btVehicleRL::updateWheelTransform(int wheelIndex) {
 	btWheelInfoRL& wheel = m_wheelInfo[wheelIndex];
 	updateWheelTransformsWS(wheel);
 	btVector3 up = -wheel.m_raycastInfo.m_wheelDirectionWS;
 	const btVector3& right = wheel.m_raycastInfo.m_wheelAxleWS;
 	btVector3 fwd = up.cross(right);
 	fwd = fwd.normalize();
@@ -99,14 +100,15 @@
 
 		wheel.m_raycastInfo.m_contactNormalWS = -wheel.m_raycastInfo.m_wheelDirectionWS;
 		wheel.m_clippedInvContactDotSuspension = 1;
 		wheel.m_extraPushback = 0;
 	}
 }
 
+// See: I20 or I21
 void btVehicleRL::updateWheelTransformsWS(btWheelInfoRL& wheel) {
 	wheel.m_raycastInfo.m_isInContact = false;
 	wheel.m_isInContactWithWorld = false;
 
 	btTransform chassisTrans = getChassisWorldTransform();
 	wheel.m_raycastInfo.m_hardPointWS = chassisTrans(wheel.m_chassisConnectionPointCS);
 	wheel.m_raycastInfo.m_wheelDirectionWS = chassisTrans.getBasis() * wheel.m_wheelDirectionCS;
@@ -117,30 +119,32 @@
 	updateWheelTransformsWS(wheel);
 
 	float depth = -1;
 
 	float suspensionTravel = wheel.m_maxSuspensionTravelCm / 100;
 	float realRayLength = wheel.getSuspensionRestLength() + suspensionTravel + wheel.m_wheelsRadius - RLConst::BTVehicle::SUSPENSION_SUBTRACTION;
 
+	// See: I21
 	btVector3 source = wheel.m_raycastInfo.m_hardPointWS;
 	btVector3 target = source + (wheel.m_raycastInfo.m_wheelDirectionWS * realRayLength);
 	wheel.m_raycastInfo.m_contactPointWS = target;
 	wheel.m_raycastInfo.m_groundObject = NULL;
 
+	// See: I22
 	btVehicleRaycaster::btVehicleRaycasterResult rayResults;
-
+	
 	btAssert(m_vehicleRaycaster);
-
 	btCollisionObject* object;
 	if (grid) {
 		object = grid->CastSuspensionRay(m_vehicleRaycaster, source, target, m_chassisBody, rayResults);
 	} else {
 		object = (btCollisionObject*)m_vehicleRaycaster->castRay(source, target, m_chassisBody, rayResults);
 	}
 
+	// See: I23
 	if (object) {
 		wheel.m_raycastInfo.m_contactPointWS = rayResults.m_hitPointInWorld;
 		float fraction = rayResults.m_distFraction;
 		depth = realRayLength * rayResults.m_distFraction;
 		wheel.m_raycastInfo.m_contactNormalWS = rayResults.m_hitNormalInWorld;
 		wheel.m_raycastInfo.m_isInContact = true;
 		wheel.m_isInContactWithWorld = object->isStaticObject();
@@ -265,17 +269,17 @@
 }
 
 void btVehicleRL::setBrake(float brake, int wheelIndex) {
 	btAssert((wheelIndex >= 0) && (wheelIndex < getNumWheels()));
 	getWheelInfo(wheelIndex).m_brake = brake;
 }
 
+// See: I24
 void btVehicleRL::updateSuspension(float deltaTime) {
-	float chassisMass = 1 / m_chassisBody->getInvMass();
-
+	
 	for (int i = 0; i < getNumWheels(); i++) {
 		btWheelInfoRL& wheel_info = m_wheelInfo[i];
 
 		if (wheel_info.m_raycastInfo.m_isInContact) {
 			float force =
 				(wheel_info.getSuspensionRestLength() - wheel_info.m_raycastInfo.m_suspensionLength)
 				* wheel_info.m_suspensionStiffness * wheel_info.m_clippedInvContactDotSuspension;
@@ -291,25 +295,25 @@
 
 		} else {
 			wheel_info.m_wheelsSuspensionForce = 0;
 		}
 	}
 
 	for (int i = 0; i < getNumWheels(); i++) {
-		//apply suspension force
 		btWheelInfoRL& wheel = m_wheelInfo[i];
 		if (wheel.m_wheelsSuspensionForce != 0) {
 			btVector3 contactPointOffset = wheel.m_raycastInfo.m_contactPointWS - getRigidBody()->getCenterOfMassPosition();
 			float baseForceScale = (wheel.m_wheelsSuspensionForce * deltaTime) + wheel.m_extraPushback;
 			btVector3 force = wheel.m_raycastInfo.m_contactNormalWS * baseForceScale;
 			m_chassisBody->applyImpulse(force, contactPointOffset);
 		}
 	}
 }
 
+// See: I25
 void btVehicleRL::calcFrictionImpulses(float timeStep) {
 
 	float frictionScale = m_chassisBody->getMass() / 3;
 
 	// Determine impulses
 	for (int i = 0; i < 4; i++) {
 		btWheelInfoRL& wheel = m_wheelInfo[i];
@@ -378,14 +382,15 @@
 			wheel.m_impulse = totalFrictionForce * frictionScale;
 		} else {
 			wheel.m_impulse = { 0,0,0 };
 		}
 	}
 }
 
+// See: I25
 void btVehicleRL::applyFrictionImpulses(float timeStep) {
 	// Apply impulses
 	btVector3 upDir = m_chassisBody->getWorldTransform().getBasis().getColumn(m_indexUpAxis);
 	for (int i = 0; i < 4; i++) {
 		btWheelInfoRL& wheel = m_wheelInfo[i];
 		if (!wheel.m_impulse.isZero()) {
 			btVector3 wheelContactOffset = wheel.m_raycastInfo.m_contactPointWS - m_chassisBody->getWorldTransform().getOrigin();
```

### Comparing `RocketSim-2.1.0a2/src/Sim/btVehicleRL/btVehicleRL.h` & `RocketSim-2.1.0a3/src/Sim/btVehicleRL/btVehicleRL.h`

 * *Files identical despite different names*

