# Comparing `tmp/opsvis-1.1.5.tar.gz` & `tmp/opsvis-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opsvis-1.1.5.tar", last modified: Mon Mar 25 14:15:08 2024, max compression
+gzip compressed data, was "opsvis-1.1.6.tar", last modified: Sun Jun  2 19:51:14 2024, max compression
```

## Comparing `opsvis-1.1.5.tar` & `opsvis-1.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 sewi      (1000) sewi      (1000)        0 2024-03-25 14:15:08.502707 opsvis-1.1.5/
--rw-r--r--   0 sewi      (1000) sewi      (1000)    35149 2020-08-24 10:31:43.000000 opsvis-1.1.5/LICENSE
--rw-r--r--   0 sewi      (1000) sewi      (1000)     1068 2024-03-25 14:15:08.502707 opsvis-1.1.5/PKG-INFO
--rw-r--r--   0 sewi      (1000) sewi      (1000)      477 2021-09-28 08:54:43.000000 opsvis-1.1.5/README.md
-drwxrwxr-x   0 sewi      (1000) sewi      (1000)        0 2024-03-25 14:15:08.502707 opsvis-1.1.5/opsvis/
--rw-r--r--   0 sewi      (1000) sewi      (1000)      154 2023-05-13 19:50:46.000000 opsvis-1.1.5/opsvis/__init__.py
--rw-r--r--   0 sewi      (1000) sewi      (1000)    20912 2023-05-14 06:27:30.000000 opsvis-1.1.5/opsvis/anim.py
--rw-r--r--   0 sewi      (1000) sewi      (1000)    47702 2023-11-10 08:58:20.000000 opsvis-1.1.5/opsvis/defo.py
--rw-r--r--   0 sewi      (1000) sewi      (1000)     9113 2024-01-29 07:45:07.000000 opsvis-1.1.5/opsvis/fibsec.py
--rw-r--r--   0 sewi      (1000) sewi      (1000)      195 2023-05-13 20:08:21.000000 opsvis-1.1.5/opsvis/importing_modules.py
--rw-r--r--   0 sewi      (1000) sewi      (1000)    75179 2024-03-25 14:12:41.000000 opsvis-1.1.5/opsvis/model.py
--rw-r--r--   0 sewi      (1000) sewi      (1000)    29911 2024-03-12 09:55:55.000000 opsvis-1.1.5/opsvis/secforces.py
--rw-r--r--   0 sewi      (1000) sewi      (1000)     4621 2023-11-10 08:58:20.000000 opsvis-1.1.5/opsvis/settings.py
--rw-r--r--   0 sewi      (1000) sewi      (1000)    34781 2023-05-13 20:08:22.000000 opsvis-1.1.5/opsvis/stress.py
-drwxrwxr-x   0 sewi      (1000) sewi      (1000)        0 2024-03-25 14:15:08.502707 opsvis-1.1.5/opsvis.egg-info/
--rw-r--r--   0 sewi      (1000) sewi      (1000)     1068 2024-03-25 14:15:08.000000 opsvis-1.1.5/opsvis.egg-info/PKG-INFO
--rw-r--r--   0 sewi      (1000) sewi      (1000)      357 2024-03-25 14:15:08.000000 opsvis-1.1.5/opsvis.egg-info/SOURCES.txt
--rw-r--r--   0 sewi      (1000) sewi      (1000)        1 2024-03-25 14:15:08.000000 opsvis-1.1.5/opsvis.egg-info/dependency_links.txt
--rw-r--r--   0 sewi      (1000) sewi      (1000)       11 2024-03-25 14:15:08.000000 opsvis-1.1.5/opsvis.egg-info/requires.txt
--rw-r--r--   0 sewi      (1000) sewi      (1000)        7 2024-03-25 14:15:08.000000 opsvis-1.1.5/opsvis.egg-info/top_level.txt
--rw-r--r--   0 sewi      (1000) sewi      (1000)      104 2021-09-23 09:12:02.000000 opsvis-1.1.5/pyproject.toml
--rw-r--r--   0 sewi      (1000) sewi      (1000)      704 2024-03-25 14:15:08.502707 opsvis-1.1.5/setup.cfg
+drwxrwxr-x   0 sewi      (1000) sewi      (1000)        0 2024-06-02 19:51:14.195102 opsvis-1.1.6/
+-rw-r--r--   0 sewi      (1000) sewi      (1000)    35149 2020-08-24 10:31:43.000000 opsvis-1.1.6/LICENSE
+-rw-r--r--   0 sewi      (1000) sewi      (1000)     1068 2024-06-02 19:51:14.195102 opsvis-1.1.6/PKG-INFO
+-rw-r--r--   0 sewi      (1000) sewi      (1000)      477 2021-09-28 08:54:43.000000 opsvis-1.1.6/README.md
+drwxrwxr-x   0 sewi      (1000) sewi      (1000)        0 2024-06-02 19:51:14.195102 opsvis-1.1.6/opsvis/
+-rw-r--r--   0 sewi      (1000) sewi      (1000)      154 2023-05-13 19:50:46.000000 opsvis-1.1.6/opsvis/__init__.py
+-rw-r--r--   0 sewi      (1000) sewi      (1000)    20912 2023-05-14 06:27:30.000000 opsvis-1.1.6/opsvis/anim.py
+-rw-r--r--   0 sewi      (1000) sewi      (1000)    47702 2023-11-10 08:58:20.000000 opsvis-1.1.6/opsvis/defo.py
+-rw-r--r--   0 sewi      (1000) sewi      (1000)     9113 2024-01-29 07:45:07.000000 opsvis-1.1.6/opsvis/fibsec.py
+-rw-r--r--   0 sewi      (1000) sewi      (1000)      195 2023-05-13 20:08:21.000000 opsvis-1.1.6/opsvis/importing_modules.py
+-rw-r--r--   0 sewi      (1000) sewi      (1000)    92246 2024-06-02 19:48:12.000000 opsvis-1.1.6/opsvis/model.py
+-rw-r--r--   0 sewi      (1000) sewi      (1000)    29911 2024-03-12 09:55:55.000000 opsvis-1.1.6/opsvis/secforces.py
+-rw-r--r--   0 sewi      (1000) sewi      (1000)     4621 2023-11-10 08:58:20.000000 opsvis-1.1.6/opsvis/settings.py
+-rw-r--r--   0 sewi      (1000) sewi      (1000)    34781 2023-05-13 20:08:22.000000 opsvis-1.1.6/opsvis/stress.py
+drwxrwxr-x   0 sewi      (1000) sewi      (1000)        0 2024-06-02 19:51:14.195102 opsvis-1.1.6/opsvis.egg-info/
+-rw-r--r--   0 sewi      (1000) sewi      (1000)     1068 2024-06-02 19:51:14.000000 opsvis-1.1.6/opsvis.egg-info/PKG-INFO
+-rw-r--r--   0 sewi      (1000) sewi      (1000)      357 2024-06-02 19:51:14.000000 opsvis-1.1.6/opsvis.egg-info/SOURCES.txt
+-rw-r--r--   0 sewi      (1000) sewi      (1000)        1 2024-06-02 19:51:14.000000 opsvis-1.1.6/opsvis.egg-info/dependency_links.txt
+-rw-r--r--   0 sewi      (1000) sewi      (1000)       11 2024-06-02 19:51:14.000000 opsvis-1.1.6/opsvis.egg-info/requires.txt
+-rw-r--r--   0 sewi      (1000) sewi      (1000)        7 2024-06-02 19:51:14.000000 opsvis-1.1.6/opsvis.egg-info/top_level.txt
+-rw-r--r--   0 sewi      (1000) sewi      (1000)      104 2021-09-23 09:12:02.000000 opsvis-1.1.6/pyproject.toml
+-rw-r--r--   0 sewi      (1000) sewi      (1000)      704 2024-06-02 19:51:14.195102 opsvis-1.1.6/setup.cfg
```

### Comparing `opsvis-1.1.5/LICENSE` & `opsvis-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `opsvis-1.1.5/PKG-INFO` & `opsvis-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opsvis
-Version: 1.1.5
+Version: 1.1.6
 Summary: OpenSeesPy (OpenSees) Python postprocessing and visualization module
 Home-page: https://github.com/sewkokot/opsvis
 Author: Seweryn Kokot
 Author-email: sewkokot@gmail.com
 Project-URL: Bug Tracker, https://github.com/sewkokot/opsvis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `opsvis-1.1.5/opsvis/anim.py` & `opsvis-1.1.6/opsvis/anim.py`

 * *Files identical despite different names*

### Comparing `opsvis-1.1.5/opsvis/defo.py` & `opsvis-1.1.6/opsvis/defo.py`

 * *Files identical despite different names*

### Comparing `opsvis-1.1.5/opsvis/fibsec.py` & `opsvis-1.1.6/opsvis/fibsec.py`

 * *Files identical despite different names*

### Comparing `opsvis-1.1.5/opsvis/model.py` & `opsvis-1.1.6/opsvis/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -473,15 +473,15 @@
         nd_crd = ops.nodeCoord(node_tag)
 
         fixed_dofs = ops.getFixedDOFs(node_tag)
 
         if ndim == 2:
             if (fixed_dofs == [1, 2, 3]):
                 m_type = path_fix
-            elif (fixed_dofs == [1, 2]):
+            elif (fixed_dofs == [1, 2] or fixed_dofs == [2, 1]):
                 m_type = path_pin
             elif (fixed_dofs == [1]):
                 m_type = path_roller_vert
             elif (fixed_dofs == [2]):
                 m_type = path_roller_horiz
 
             ax.plot(nd_crd[0], nd_crd[1], marker=m_type, markersize=m_size,
@@ -1598,14 +1598,427 @@
 
     ax.axis('equal')
     ax.grid(False)
 
     return ax
 
 
+def plot_loads_3d(nep=11, sfac=False, fig_wi_he=False,
+                  fig_lbrt=False, fmt_model_loads=fmt_model_loads,
+                  node_supports=True, truss_node_offset=0, ax=False):
+    """Display the nodal and element loads applied to the 2d models.
+
+    Args:
+        nep (int): number of arrows when displacing element distributed loads
+            (default: 11)
+
+        node_supports (bool): True - show the node support conditions.
+            Default: False.
+
+    """
+
+    if not ax:
+        if fig_wi_he:
+            fig_wi, fig_he = fig_wi_he
+
+            fig = plt.figure(figsize=(fig_wi / 2.54, fig_he / 2.54))
+
+        else:
+            fig = plt.figure()
+
+        if fig_lbrt:
+            fleft, fbottom, fright, ftop = fig_lbrt
+            fig.subplots_adjust(left=fleft, bottom=fbottom, right=fright, top=ftop)
+
+        ax = fig.add_subplot(111, projection=Axes3D.name)
+
+    ax = plot_model(node_labels=0, element_labels=0, fmt_model=fmt_model_loads,
+                    node_supports=node_supports, local_axes=local_axes, ax=ax)
+    # ax.axis('equal')
+
+    if not sfac:
+        ratio = 0.1
+        min_x, max_x = ax.get_xlim()
+        min_y, max_y = ax.get_ylim()
+        min_z, max_z = ax.get_zlim()
+        xsfac = ratio * abs(max_x - min_x)
+        ysfac = ratio * abs(max_y - min_y)
+        zsfac = ratio * abs(max_z - min_z)
+        sfac = max(xsfac, ysfac, zsfac)
+
+    node_tags = ops.getNodeTags()
+    ele_tags = ops.getEleTags()
+    # ndf = ops.getNDF()[0]
+
+    Wx = False
+    waa = False
+    wab = False
+
+    # get Ew data
+    Ew = get_Ew_data_from_ops_domain_3d()
+
+    for ele_tag in ele_tags:  # plot load 3d
+
+        ele_class_tag = ops.getEleClassTags(ele_tag)[0]
+
+        if (ele_class_tag == EleClassTag.ElasticBeam3d
+            or ele_class_tag == EleClassTag.ForceBeamColumn3d
+            or ele_class_tag == EleClassTag.DispBeamColumn3d):
+
+            # by default no element load
+            ele_load_data = []
+            if ele_tag in Ew:
+                ele_load_data = Ew[ele_tag]
+
+            nen = 2
+            ele_node_tags = ops.eleNodes(ele_tag)
+            ecrd_nodes = np.zeros((nen, 3))
+            for i, ele_node_tag in enumerate(ele_node_tags):
+                ecrd_nodes[i, :] = ops.nodeCoord(ele_node_tag)
+
+            ecrd_eles = np.copy(ecrd_nodes)
+
+            ele_offsets = np.array(ops.eleResponse(ele_tag, 'offsets'))
+            nz_offsets = np.nonzero(ele_offsets)[0]  # tuple of arrays
+            if np.any(nz_offsets):  # plot load 3d
+                # modify ecrd_eles
+                ecrd_eles[:, 0] += ele_offsets[[0, 3]]
+                ecrd_eles[:, 1] += ele_offsets[[1, 4]]
+                ecrd_eles[:, 2] += ele_offsets[[2, 5]]
+            else:
+                pass
+
+            # step 1: first plot model itself
+            # ax.plot(ex, ey, 'k-', solid_capstyle='round', solid_joinstyle='round',
+            #         dash_capstyle='butt', dash_joinstyle='round')
+
+            # step 2
+            xloc = ops.eleResponse(ele_tag, 'xlocal')
+            yloc = ops.eleResponse(ele_tag, 'ylocal')
+            zloc = ops.eleResponse(ele_tag, 'zlocal')
+            g = np.vstack((xloc, yloc, zloc))
+
+            G, L = rot_transf_3d(ecrd_eles, g)
+
+            xl = np.linspace(0., L, nep)
+            xl2 = np.linspace(0., L, 5)
+            # xl2 = np.logspace(0., 1., nep) * L / nep
+            dxs = np.array([0.1, 0.2, 0.3, 0.4])
+            # dxs = np.array([0.15, 0.2, 0.275, 0.375])
+            xl3 = np.append(0., np.cumsum(dxs)) * L
+
+            one = np.ones(nep)
+
+            for ele_load_data_i in ele_load_data:  # plot load 3d
+                ele_load_type = ele_load_data_i[0]
+
+                # fixme uncomment when regular uniformLoad works! (1)
+                if ele_load_type == '-beamPoint':  # plot load 3d
+                    Py, Pz, aL, Px = ele_load_data_i[1:5]
+                    Pyzx = [Px, Py, Pz]
+                    xa = aL * L
+                    text_string = f'Pyzx:{Py},{Pz},{Px}'
+
+                    s_0 = np.zeros(3)
+                    s_0[0] = ecrd_eles[0, 0] + xa * g[0, 0]
+                    s_0[1] = ecrd_eles[0, 1] + xa * g[0, 1]
+                    s_0[2] = ecrd_eles[0, 2] + xa * g[0, 2]
+
+                    for k, Pi in enumerate(Pyzx):
+
+                        if Pi != 0:
+                            dir_plt = k
+                            s = sfac * np.sign(Pi)
+
+                            s_p = np.copy(s_0)
+
+                            s_p[0] += s * g[dir_plt, 0]
+                            s_p[1] += s * g[dir_plt, 1]
+                            s_p[2] += s * g[dir_plt, 2]
+
+                            nn = 2
+                            ax.arrow3D(s_0[0], s_0[1], s_0[2],
+                                       nn * (s_p[0] - s_0[0]),
+                                       nn * (s_p[1] - s_0[1]),
+                                       nn * (s_p[2] - s_0[2]), mutation_scale=8)
+
+                        ax.text(s_0[0], s_0[1], s_0[2],
+                                text_string, va='bottom', ha='center', color='r')
+
+                elif ele_load_type == '-beamUniform':  # plot load 3d
+
+                    n_ele_load_data = len(ele_load_data_i)
+
+                    if n_ele_load_data == 4:
+                        Wy, Wz, Wx = ele_load_data_i[1:4]
+                        text_string = f'q = {Wy}, {Wz}, {Wx}'
+                        Wxyz = [Wx, Wy, Wz]
+
+                        s_0 = np.zeros((nep, 3))
+                        s_0[0, :] = [ecrd_eles[0, 0], ecrd_eles[0, 1], ecrd_eles[0, 2]]
+
+                        # fixme
+                        s_0[1:, 0] = s_0[0, 0] + xl[1:] * g[0, 0]
+                        s_0[1:, 1] = s_0[0, 1] + xl[1:] * g[0, 1]
+                        s_0[1:, 2] = s_0[0, 2] + xl[1:] * g[0, 2]
+
+                        for k, Wi in enumerate(Wxyz):
+
+                            if Wi != 0:
+
+                                dir_plt = k
+                                s = sfac * one * np.sign(Wi)
+                                s = s * sfac
+
+                                s_p = np.copy(s_0)
+
+                                # s_p[:, 0] -= s * g[dir_plt, 0]
+                                s_p[:, 0] += s * g[dir_plt, 0]
+                                s_p[:, 1] += s * g[dir_plt, 1]
+                                s_p[:, 2] += s * g[dir_plt, 2]
+
+                                if k == 0:
+                                    nn = 1
+                                else:
+                                    nn = 4
+
+                                for i in np.arange(nep):
+                                    ax.arrow3D(s_0[i, 0], s_0[i, 1], s_0[i, 2],
+                                               nn * (s_p[i, 0] - s_0[i, 0]),
+                                               nn * (s_p[i, 1] - s_0[i, 1]),
+                                               nn * (s_p[i, 2] - s_0[i, 2]), mutation_scale=8)
+
+                            ax.text(sum(ecrd_eles[:, 0]) / 2,
+                                    sum(ecrd_eles[:, 1]) / 2,
+                                    sum(ecrd_eles[:, 2]) / 2,
+                                    text_string, va='bottom', ha='center', color='r')
+
+                    # triangular or trapezoidal element load
+                    elif n_ele_load_data == 7:
+                        wta, waa, aL, bL, wtb, wab = ele_load_data_i[1:7]
+                        text_string = f'q = {wta}, {waa}, {aL}, {bL}, {wtb}, {wab}'
+                        a, b = aL * L, bL * L
+                        bma = b - a
+                        s = np.zeros(nep)
+
+                        indx = 0
+                        for x in np.nditer(xl):
+                            xma = x - a
+                            wtx = wta + (wtb - wta) * xma / bma
+
+                            if x < a:
+                                pass
+                            elif x >= a and x <= b:
+                                s[indx] = wtx
+                            elif x > b:
+                                pass
+
+                            indx += 1
+
+                    # if Wx != 0:
+                    #     # for i, xl in enumerate(xl2[:-1]):
+                    #     #     plt.arrow(sa[i, 0], sa[i, 1],
+                    #     #               sa[i+1, 0]-sa[i, 0], sa[i+1, 1]-sa[i, 1],
+                    #     #               width = 0.01,
+                    #     #               # lw = 1,
+                    #     #               # head_width=0.02, head_length=0.05,
+                    #     #               # head_starts_at_zero=True,  # default False
+                    #     #               # overhang=0.5,
+                    #     #               fc='m', ec='m',
+                    #     #               length_includes_head=True, shape='full')
+
+                    #     ax.quiver(s_0[:-1, 0], s_0[:-1, 1],
+                    #               s_0[1:, 0]-s_0[:-1, 0], s_0[1:, 1]-s_0[:-1, 1],
+                    #               scale_units='xy', angles='xy', scale=0.8, color='m')
+
+                    # if waa != 0 or wab != 0:
+                    #     sa = np.zeros((5, 2))
+                    #     sa[0, :] = [ex[0], ey[0]]
+                    #     sa[1:, 0] = sa[0, 0] + xl3[1:] * cosa
+                    #     sa[1:, 1] = sa[0, 1] + xl3[1:] * cosb
+
+                    #     for i, xl in enumerate(xl3[:-1]):
+                    #         ax.arrow(sa[i, 0], sa[i, 1],
+                    #                  sa[i+1, 0]-sa[i, 0], sa[i+1, 1]-sa[i, 1],
+                    #                  # width = 0.05,
+                    #                  width = 0.01*L,
+                    #                  # lw = 1,
+                    #                  # head_width=0.02, head_length=0.05,
+                    #                  # head_starts_at_zero=True,  # default False
+                    #                  # overhang=0.5,
+                    #                  fc='m', ec='m',
+                    #                  length_includes_head=True, shape='full')
+
+                    #     # ax.quiver(sa[:-1, 0], sa[:-1, 1],
+                    #     #            sa[1:, 0]-sa[:-1, 0], sa[1:, 1]-sa[:-1, 1],
+                    #     #            scale_units='xy', angles='xy', scale=0.8, color='g')
+
+                    #     # ax.plot([s_0[i, 0], s_p[i, 0]], [s_0[i, 1], s_p[i, 1]],
+                    #     #          fmt_secforce, solid_capstyle='round',
+                    #     #          solid_joinstyle='round', dash_capstyle='butt',
+                    #     #          dash_joinstyle='round')
+                    #     # plot arrows
+                    #     # ax.annotate("",
+                    #     #              xy=(s_p[i, 0], s_p[i, 1]), xycoords='data',
+                    #     #              xytext=(s_0[i, 0], s_0[i, 1]), textcoords='data',
+                    #     #              arrowprops=dict(arrowstyle="->", color='r', lw=2,
+                    #     #                              connectionstyle="arc3"))
+
+    for node_tag in node_tags:
+        nd_crd = ops.nodeCoord(node_tag)
+
+        nodal_loads = ops.nodeUnbalance(node_tag)  # plot load 3d
+        nodal_loads_idx = np.nonzero(nodal_loads)
+
+        if nodal_loads_idx[0].size:
+            for kier in nodal_loads_idx[0]:
+                if kier == 0 or kier == 1 or kier == 2 or kier == 3 or kier == 4 or kier == 5:
+                    if kier == 0:
+                        kier2 = np.sign(nodal_loads[kier])
+                        if kier2 > 0:
+                            pos_or_neg = '+'
+                        elif kier2 < 0:
+                            pos_or_neg = '-'
+                        dx = sfac * np.sign(kier2)
+                        dy = 0.
+                        dz = 0.
+                        kolor = 'b'
+
+                    elif kier == 1:
+                        kier2 = np.sign(nodal_loads[kier])
+                        if kier2 > 0:
+                            pos_or_neg = '+'
+                        elif kier2 < 0:
+                            pos_or_neg = '-'
+                        dx = 0.
+                        dy = sfac * np.sign(kier2)
+                        dz = 0.
+                        kolor = 'b'
+
+                    elif kier == 2:
+                        kier2 = np.sign(nodal_loads[kier])
+                        if kier2 > 0:
+                            pos_or_neg = '+'
+                        elif kier2 < 0:
+                            pos_or_neg = '-'
+                        dx = 0.
+                        dy = 0.
+                        dz = sfac * np.sign(kier2)
+                        kolor = 'b'
+
+                    elif kier == 3:
+                        kier2 = np.sign(nodal_loads[kier])
+                        if kier2 > 0:
+                            pos_or_neg = '+'
+                        elif kier2 < 0:
+                            pos_or_neg = '-'
+                        dx = sfac * np.sign(kier2)
+                        dy = 0.
+                        dz = 0.
+                        kolor = 'r'
+
+                    elif kier == 4:
+                        kier2 = np.sign(nodal_loads[kier])
+                        if kier2 > 0:
+                            pos_or_neg = '+'
+                        elif kier2 < 0:
+                            pos_or_neg = '-'
+                        dx = 0.
+                        dy = sfac * np.sign(kier2)
+                        dz = 0.
+                        kolor = 'r'
+
+                    elif kier == 5:
+                        kier2 = np.sign(nodal_loads[kier])
+                        if kier2 > 0:
+                            pos_or_neg = '+'
+                        elif kier2 < 0:
+                            pos_or_neg = '-'
+                        dx = 0.
+                        dy = 0.
+                        dz = sfac * np.sign(kier2)
+                        kolor = 'r'
+
+                    ax.quiver(nd_crd[0], nd_crd[1], nd_crd[2],
+                              dx, dy, dz, length=2.0, color=kolor)
+                    if kier == 3 or kier == 4 or kier == 5:
+                        ax.quiver(nd_crd[0] + dx, nd_crd[1] + dy, nd_crd[2] + dz,
+                                  1.5 * dx, 1.5 * dy, 1.5 * dz, length=1.0, color=kolor)
+                    # ar1 = Arrow3D([nd_crd[0], nd_crd[0]+dx], [nd_crd[1], nd_crd[1]+dy], [nd_crd[2], nd_crd[2]+dz], mutation_scale=20,
+                    #               lw=1, arrowstyle="-|>", color="k")
+                    # ar1 = Arrow3D(nd_crd[0], nd_crd[1], nd_crd[2], dx, dy, dz)
+
+                    # ax.add_artist(ar1)
+                    # ax.arrow3D(0,0,0,1,1,1, mutation_scale=20,
+                    #            arrowstyle="-|>")
+                    # ax.arrow3D(nd_crd[0], nd_crd[1], nd_crd[2],
+                    #            dx, dy, dz)
+
+                    # ax.arrow3D(nd_crd[0], nd_crd[1], nd_crd[2],
+                    #            dx, dy, dz, mutation_scale=15,
+                    #            arrowstyle="-|>",
+                    #            ec='blue', fc='blue')
+
+                    #            # width = 0.01,
+                    #            head_starts_at_zero=True,  # default False
+                    #            overhang=0.2,
+                    #            lw=3,
+                    #            head_width=0.1*sfac, head_length=0.2*sfac,
+                    #            fc='b', ec='b',
+                    #            length_includes_head=True, shape='full')
+                    # ax.text(nd_crd[0]+dx, nd_crd[1]+dy, f' {nodal_loads[kier]:.5g}', color='b')
+
+                # concentrated bending moment
+                elif kier == 2:
+                    kier2 = np.sign(nodal_loads[kier])
+                    if kier2 > 0:
+                        pos_or_neg = 'anti-clockwise'
+                        # marker_type=r'$\circlearrowleft$'
+                        marker_type = r'$\curvearrowleft$'
+                    elif kier2 < 0:
+                        pos_or_neg = 'clockwise'
+                        # marker_type=r'$\circlearrowright$'
+                        marker_type = r'$\curvearrowright$'
+
+                    ax.plot(nd_crd[0], nd_crd[1], marker=marker_type, markersize=35, color='b')
+                    ax.text(nd_crd[0], nd_crd[1], f'{nodal_loads[kier]:.5g}', color='b', va='bottom', ha='left')
+
+    # ax.axis('equal')
+    # ax.grid(False)
+
+    return ax
+
+
+def plot_load(nep=11, sfac=False, fig_wi_he=False,
+              fig_lbrt=False, fmt_model_loads=fmt_model_loads,
+              node_supports=True, truss_node_offset=0, ax=False):
+    """
+    Plot loads for 2d and 3d models
+    """
+    ndim = ops.getNDM()[0]
+
+    if ndim == 2:
+        ax = plot_loads_2d(nep, sfac, fig_wi_he,
+                           fig_lbrt, fmt_model_loads,
+                           node_supports, truss_node_offset, ax)
+
+    elif ndim == 3:
+        ax = plot_loads_3d(nep, sfac, fig_wi_he,
+                           fig_lbrt, fmt_model_loads,
+                           node_supports, truss_node_offset, ax)
+
+    # elif ndim == 1:
+    #     ax = plot_loads_1d()
+
+    else:
+        print(f'\nWarning! ndim: {ndim} not supported yet.')
+
+    return ax
+
+
 def get_nodal_loads_from_ops_domain():
     load_at_nodes = {}
     ibeg, iend = 0, 0
 
     node_load_tags_all_patterns = ops.getNodeLoadTags()
     node_load_data_all_patterns = ops.getNodeLoadData()
```

### Comparing `opsvis-1.1.5/opsvis/secforces.py` & `opsvis-1.1.6/opsvis/secforces.py`

 * *Files identical despite different names*

### Comparing `opsvis-1.1.5/opsvis/settings.py` & `opsvis-1.1.6/opsvis/settings.py`

 * *Files identical despite different names*

### Comparing `opsvis-1.1.5/opsvis/stress.py` & `opsvis-1.1.6/opsvis/stress.py`

 * *Files identical despite different names*

### Comparing `opsvis-1.1.5/opsvis.egg-info/PKG-INFO` & `opsvis-1.1.6/opsvis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opsvis
-Version: 1.1.5
+Version: 1.1.6
 Summary: OpenSeesPy (OpenSees) Python postprocessing and visualization module
 Home-page: https://github.com/sewkokot/opsvis
 Author: Seweryn Kokot
 Author-email: sewkokot@gmail.com
 Project-URL: Bug Tracker, https://github.com/sewkokot/opsvis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `opsvis-1.1.5/setup.cfg` & `opsvis-1.1.6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = opsvis
-version = 1.1.5
+version = 1.1.6
 author = Seweryn Kokot
 author_email = sewkokot@gmail.com
 description = OpenSeesPy (OpenSees) Python postprocessing and visualization module
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sewkokot/opsvis
 project_urls =
```

