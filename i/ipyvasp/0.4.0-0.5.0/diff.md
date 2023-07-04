# Comparing `tmp/ipyvasp-0.4.0.tar.gz` & `tmp/ipyvasp-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyvasp-0.4.0.tar", last modified: Sun Jul  2 19:27:38 2023, max compression
+gzip compressed data, was "ipyvasp-0.5.0.tar", last modified: Tue Jul  4 17:30:06 2023, max compression
```

## Comparing `ipyvasp-0.4.0.tar` & `ipyvasp-0.5.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 19:27:38.169940 ipyvasp-0.4.0/
--rw-rw-rw-   0        0        0     1263 2023-02-22 21:17:10.000000 ipyvasp-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     1862 2023-07-02 19:27:38.169940 ipyvasp-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1228 2023-06-24 22:17:33.000000 ipyvasp-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 19:27:38.083671 ipyvasp-0.4.0/ipyvasp/
--rw-rw-rw-   0        0        0     1844 2023-07-02 19:12:11.000000 ipyvasp-0.4.0/ipyvasp/__init__.py
--rw-rw-rw-   0        0        0    38535 2023-06-26 16:58:40.000000 ipyvasp-0.4.0/ipyvasp/_enplots.py
--rw-rw-rw-   0        0        0    88362 2023-07-02 19:00:28.000000 ipyvasp-0.4.0/ipyvasp/_lattice.py
--rw-rw-rw-   0        0        0       23 2023-07-02 19:26:08.000000 ipyvasp-0.4.0/ipyvasp/_version.py
--rw-rw-rw-   0        0        0    30580 2023-06-25 15:31:44.000000 ipyvasp-0.4.0/ipyvasp/bsdos.py
--rw-rw-rw-   0        0        0     2712 2023-06-24 19:19:43.000000 ipyvasp-0.4.0/ipyvasp/cli.py
-drwxrwxrwx   0        0        0        0 2023-07-02 19:27:38.160705 ipyvasp-0.4.0/ipyvasp/core/
--rw-rw-rw-   0        0        0        0 2023-06-24 01:13:48.000000 ipyvasp-0.4.0/ipyvasp/core/__init__.py
--rw-rw-rw-   0        0        0    37726 2023-07-02 17:25:50.000000 ipyvasp-0.4.0/ipyvasp/core/parser.py
--rw-rw-rw-   0        0        0    34144 2023-07-01 01:10:51.000000 ipyvasp-0.4.0/ipyvasp/core/plot_toolkit.py
--rw-rw-rw-   0        0        0    28883 2023-07-01 23:07:24.000000 ipyvasp-0.4.0/ipyvasp/core/serializer.py
--rw-rw-rw-   0        0        0    11706 2023-07-01 21:50:03.000000 ipyvasp-0.4.0/ipyvasp/core/spatial_toolkit.py
--rw-rw-rw-   0        0        0    19335 2023-07-02 18:12:36.000000 ipyvasp-0.4.0/ipyvasp/evals_dataframe.py
--rw-rw-rw-   0        0        0    25929 2023-07-02 19:05:49.000000 ipyvasp-0.4.0/ipyvasp/lattice.py
--rw-rw-rw-   0        0        0     1317 2023-06-25 00:23:12.000000 ipyvasp-0.4.0/ipyvasp/misc.py
--rw-rw-rw-   0        0        0    11406 2023-07-02 18:28:53.000000 ipyvasp-0.4.0/ipyvasp/potential.py
--rw-rw-rw-   0        0        0    15160 2023-07-01 23:51:05.000000 ipyvasp-0.4.0/ipyvasp/utils.py
--rw-rw-rw-   0        0        0    44823 2023-07-01 01:09:38.000000 ipyvasp-0.4.0/ipyvasp/widgets.py
-drwxrwxrwx   0        0        0        0 2023-07-02 19:27:38.147929 ipyvasp-0.4.0/ipyvasp.egg-info/
--rw-rw-rw-   0        0        0     1862 2023-07-02 19:27:37.000000 ipyvasp-0.4.0/ipyvasp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2023-07-02 19:27:37.000000 ipyvasp-0.4.0/ipyvasp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 19:27:37.000000 ipyvasp-0.4.0/ipyvasp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      190 2023-07-02 19:27:37.000000 ipyvasp-0.4.0/ipyvasp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-02 19:27:37.000000 ipyvasp-0.4.0/ipyvasp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 19:27:38.169940 ipyvasp-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     3676 2023-07-02 19:25:02.000000 ipyvasp-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:06.805501 ipyvasp-0.5.0/
+-rw-rw-rw-   0        0        0     1263 2023-02-22 21:17:10.000000 ipyvasp-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     1862 2023-07-04 17:30:06.804495 ipyvasp-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1228 2023-06-24 22:17:33.000000 ipyvasp-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:06.767725 ipyvasp-0.5.0/ipyvasp/
+-rw-rw-rw-   0        0        0     1707 2023-07-02 21:08:59.000000 ipyvasp-0.5.0/ipyvasp/__init__.py
+-rw-rw-rw-   0        0        0    37503 2023-07-02 21:24:03.000000 ipyvasp-0.5.0/ipyvasp/_enplots.py
+-rw-rw-rw-   0        0        0    92905 2023-07-04 17:23:48.000000 ipyvasp-0.5.0/ipyvasp/_lattice.py
+-rw-rw-rw-   0        0        0       23 2023-07-04 17:29:24.000000 ipyvasp-0.5.0/ipyvasp/_version.py
+-rw-rw-rw-   0        0        0    30580 2023-06-25 15:31:44.000000 ipyvasp-0.5.0/ipyvasp/bsdos.py
+-rw-rw-rw-   0        0        0      565 2023-07-02 21:39:58.000000 ipyvasp-0.5.0/ipyvasp/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:06.803496 ipyvasp-0.5.0/ipyvasp/core/
+-rw-rw-rw-   0        0        0        0 2023-06-24 01:13:48.000000 ipyvasp-0.5.0/ipyvasp/core/__init__.py
+-rw-rw-rw-   0        0        0    37726 2023-07-02 17:25:50.000000 ipyvasp-0.5.0/ipyvasp/core/parser.py
+-rw-rw-rw-   0        0        0    34144 2023-07-01 01:10:51.000000 ipyvasp-0.5.0/ipyvasp/core/plot_toolkit.py
+-rw-rw-rw-   0        0        0    30024 2023-07-04 17:22:33.000000 ipyvasp-0.5.0/ipyvasp/core/serializer.py
+-rw-rw-rw-   0        0        0    14743 2023-07-04 17:24:40.000000 ipyvasp-0.5.0/ipyvasp/core/spatial_toolkit.py
+-rw-rw-rw-   0        0        0    19335 2023-07-02 18:12:36.000000 ipyvasp-0.5.0/ipyvasp/evals_dataframe.py
+-rw-rw-rw-   0        0        0    22391 2023-07-03 16:19:41.000000 ipyvasp-0.5.0/ipyvasp/lattice.py
+-rw-rw-rw-   0        0        0     1317 2023-06-25 00:23:12.000000 ipyvasp-0.5.0/ipyvasp/misc.py
+-rw-rw-rw-   0        0        0    11406 2023-07-02 18:28:53.000000 ipyvasp-0.5.0/ipyvasp/potential.py
+-rw-rw-rw-   0        0        0    15160 2023-07-01 23:51:05.000000 ipyvasp-0.5.0/ipyvasp/utils.py
+-rw-rw-rw-   0        0        0    44823 2023-07-01 01:09:38.000000 ipyvasp-0.5.0/ipyvasp/widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:06.799100 ipyvasp-0.5.0/ipyvasp.egg-info/
+-rw-rw-rw-   0        0        0     1862 2023-07-04 17:30:06.000000 ipyvasp-0.5.0/ipyvasp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2023-07-04 17:30:06.000000 ipyvasp-0.5.0/ipyvasp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 17:30:06.000000 ipyvasp-0.5.0/ipyvasp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-04 17:30:06.000000 ipyvasp-0.5.0/ipyvasp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      190 2023-07-04 17:30:06.000000 ipyvasp-0.5.0/ipyvasp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-04 17:30:06.000000 ipyvasp-0.5.0/ipyvasp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-04 17:30:06.805501 ipyvasp-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     3820 2023-07-02 21:35:36.000000 ipyvasp-0.5.0/setup.py
```

### Comparing `ipyvasp-0.4.0/LICENSE` & `ipyvasp-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.4.0/PKG-INFO` & `ipyvasp-0.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyvasp
-Version: 0.4.0
+Version: 0.5.0
 Summary: A processing tool for VASP DFT input/output processing in Jupyter Notebook.
 Home-page: https://github.com/massgh/ipyvasp
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyvasp/issues
 Keywords: Jupyter,Widgets,IPython,VASP,DFT
```

### Comparing `ipyvasp-0.4.0/README.md` & `ipyvasp-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.4.0/ipyvasp/__init__.py` & `ipyvasp-0.5.0/ipyvasp/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -59,14 +59,8 @@
                 "#FF6692",
                 "#B6E880",
                 "#FF97FF",
                 "#FECB52",
             ]
         ),
     }
-)
-
-
-def docs():
-    from IPython.display import Markdown
-
-    return Markdown("[ipyvasp-docs](https://massgh.github.io/ipyvasp/)")
+)
```

### Comparing `ipyvasp-0.4.0/ipyvasp/_enplots.py` & `ipyvasp-0.5.0/ipyvasp/_enplots.py`

 * *Files 2% similar despite different names*

```diff
@@ -893,14 +893,15 @@
             range=[min(K), max(K)],
         ),
         font=dict(family="stix, serif", size=14),
     )
     return fig
 
 
+@gu._fmt_doc(_docs)
 def iplot_rgb_lines(
     K,
     E,
     pros,
     labels,
     occs,
     kpoints,
@@ -909,39 +910,25 @@
     kticks=None,
     interp=None,
     maxwidth=10,
     mode="markers + lines",
     title=None,
     **kwargs,
 ):
-    """
-    Interactive plot of band structure with rgb data points using plotly.
-
-    Parameters
-    ----------
-    K : array-like, shape (nk,)
-    E : array-like, shape (nk,nb)
-    pros : array-like, shape (m,nk,nb), m is the number of projections
-    labels : list of str, length m
+    """Interactive plot of band structure with rgb data points using plotly.
+    {params}\n    {K}\n    {E}\n    {pros}\n    {labels}\n    {elim}\n    {kticks}\n    {interp}
     occs : array-like, shape (nk,nb)
     kpoints : array-like, shape (nk,3)
     fig : plotly.graph_objects.Figure, if not provided, a new figure will be created
-    elim : tuple, (emin,emax), energy range to plot
-    kticks : [(int, str),...] for indices of high symmetry k-points. To join a broken path, use '<=' before symbol, e.g.  [(0, 'G'),(40, '<=K|M'), ...] will join 40 back to 39. You can also use shortcut like zip([0,10,20],'GMK').
-    interp : int or list/tuple of (n,k) for interpolation. If int, n is number of points to interpolate. If list/tuple, n is number of points and k is the order of spline.
     maxwidth : float, maximum linewidth, 10 by default
     mode : str, plotly mode, 'markers + lines' by default, see modes in `plotly.graph_objects.Scatter`.
     title : str, title of the figure, labels are added to the end of the title.
 
     kwargs are passed to `plotly.graph_objects.Scatter`.
-
-    Returns
-    -------
-    fig : plotly.graph_objects.Figure that can be displayed in Jupyter notebook or saved as html using `ipyvasp.iplot2html`.
-    """
+    {return_fig}"""
     if isinstance(K, dict):  # Provided by Bands class, don't do is yourself
         K, indices = K["K"], K["indices"]
     else:
         K, indices = K, range(np.shape(E)[1])  # Assume K is provided by user
 
     K, E, xticks, xticklabels = _validate_data(K, E, elim, kticks, interp)
     data = _format_rgb_data(
@@ -1014,29 +1001,26 @@
 
     Parameters
     ----------
     energy : array-like, shape (n,)
     dos_arrays : list of array_like, each of shape (n,) or array-like (m,n)
     labels : list of str, length = len(dos_arrays) should hold.
     fig : plotly.graph_objects.Figure, if not provided, a new figure will be created
-    elim : list of length 2, (emin, emax), if None, (min(energy), max(energy)) is used.
-    colormap : str, default 'tab10', any valid matplotlib colormap name. Note that colormap is take from matplotlib, not plotly.
+    {elim}
+    {colormap}
     colors : list of str, length = len(dos_arrays) should hold if given, and will override colormap. Should be valid CSS colors.
     fill : bool, default True, if True, fill the area under the DOS lines.
     vertical : bool, default False, if True, plot DOS lines vertically.
     mode : str, default 'lines', plotly mode, see modes in `plotly.graph_objects.Scatter`.
     stack : bool, default False, if True, stack the DOS lines. Only works for horizontal plots.
-    interp : int or list/tuple of (n,k), default None, if given, interpolate the DOS lines using spline.
+    {interp}
 
-    keyword arguments are passed to `plotly.graph_objects.Scatter`.
 
-    Returns
-    -------
-    fig : plotly.graph_objects.Figure
-    """
+    keyword arguments are passed to `plotly.graph_objects.Scatter`.
+    {return_fig}"""
     energy, dos_arrays, labels, colors = _fix_dos_data(
         energy, dos_arrays, labels, colors, interp
     )
     if fig is None:
         fig = go.Figure()
         fig.update_layout(
             margin=go.layout.Margin(l=60, r=50, b=40, t=75, pad=0),
```

### Comparing `ipyvasp-0.4.0/ipyvasp/_lattice.py` & `ipyvasp-0.5.0/ipyvasp/_lattice.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     to_plane,
     rotation,
     inside_convexhull,
     to_basis,
     to_R3,
     get_TM,
     get_bz,
+    coplanar,
 )
 from .core.plot_toolkit import quiver3d
 
 
 # These colors are taken from Mathematica's ColorData["Atoms"]
 _atom_colors = {
     "H": (0.7, 0.8, 0.7),
@@ -840,36 +841,40 @@
 
 # Cell
 def splot_bz(
     bz_data,
     plane=None,
     ax=None,
     color="blue",
-    fill=True,
+    fill=False,
+    fill_zorder=0,
     vectors=(0, 1, 2),
     colormap=None,
     shade=True,
     alpha=0.4,
     zoffset=0,
     **kwargs,
 ):
-    """Plots matplotlib's static figure of Brillouin zone. You can also plot in 2D on a 3D axes.
+    """Plots matplotlib's static figure of BZ/Cell. You can also plot in 2D on a 3D axes.
 
     Parameters
     ----------
     bz_data : Output of `get_bz`.
     plane : str
         Default is None and plots 3D surface. Can take 'xy','yz','zx' to plot in 2D.
     fill : bool
         True by defult, determines whether to fill surface of BZ or not.
+    fill_zorder : int
+        Default is 0, determines zorder of filled surface in 2D plots if `fill=True`.
     color : Any
         Color to fill surface and stroke color. Default is 'blue'. Can be any valid matplotlib color.
     vectors : tuple
         Tuple of indices of basis vectors to plot. Default is (0,1,2). All three are plotted in 3D
         (you can turn of by None or empty tuple), whhile you can specify any two/three in 2D.
+        Vectors do not appear if given data is subzone data.
     ax : matplotlib.pyplot.Axes
         Auto generated by default, 2D/3D axes, auto converts in 3D on demand as well.
     colormap : str
         If None, single color is applied, only works in 3D and `fill=True`. Colormap is applied along z.
     shade : bool
         Shade polygons or not. Only works in 3D and `fill=True`.
     alpha : float
@@ -882,38 +887,36 @@
 
     Returns
     -------
     matplotlib.pyplot.Axes
         Matplotlib's 2D axes if `plane=None` otherswise 3D axes.
     """
     vname = "a" if bz_data.__class__.__name__ == "CellData" else "b"
-    if vname == "b":  # These needed for splot_kpath internally
-        type(bz_data)._splot_kws = dict(plane=plane, zoffset=zoffset)
-
     label = r"$k_{}/2π$" if vname == "b" else "{}"
-    if not ax:  # For both 3D and 2D, initialize 2D axis.
-        ax = ptk.get_axes(figsize=(3.4, 3.4))  # For better display
 
-    type(bz_data)._splot_kws["ax"] = ax  # For splot_kpath
     _label = r"\vec{" + vname + "}"  # For both
 
     if vectors and not isinstance(vectors, (tuple, list)):
         raise ValueError(f"`vectors` expects tuple or list, got {vectors!r}")
 
     if vectors is None:
         vectors = ()  # Empty tuple to make things work below
 
     for v in vectors:
         if v not in [0, 1, 2]:
             raise ValueError(f"`vectors` expects values in [0,1,2], got {vectors!r}")
 
     name = kwargs.pop("label", None)  # will set only on single line
-    kwargs.pop("zdir", None)  # 2D plot on 3D axes is only supported in xy plane.
+    kwargs.pop("zdir", None)  # remove , no need
+    is_subzone = hasattr(bz_data, "_specials")  # For subzone
 
     if plane:  # Project 2D, works on 3D axes as well
+        if not ax:  # Create 2D axes if not given
+            ax = ptk.get_axes(figsize=(3.4, 3.4))  # For better display
+
         kwargs = {"solid_capstyle": "round", **kwargs}
         is3d = getattr(ax, "name", "") == "3d"
         normals = {
             "xy": (0, 0, 1),
             "yz": (1, 0, 0),
             "zx": (0, 1, 0),
             "yx": (0, 0, -1),
@@ -944,15 +947,36 @@
             g = to_plane(normals[plane], f) + z0
             (line,) = ax.plot(
                 *(g.T if is3d else g[:, idxs[plane]].T), color=color, **kwargs
             )
             if idx == 0:
                 line.set_label(name)  # only one line
 
-        if vectors:
+            if fill and not is3d:
+                ax.fill(
+                    *g[:, idxs[plane]].T,
+                    facecolor=color,
+                    edgecolor=color,
+                    linewidth=0.0001,
+                    alpha=alpha,
+                    zorder=fill_zorder,
+                )
+            elif fill and is3d:
+                poly = Poly3DCollection(
+                    [g],  # 3D fill in plane
+                    edgecolors=[color],
+                    facecolors=[color],
+                    alpha=alpha,
+                    shade=shade,
+                    zorder=fill_zorder,
+                )
+                ax.add_collection(poly)
+                ax.autoscale_view()
+
+        if vectors and not is_subzone:
             s_basis = to_plane(normals[plane], bz_data.basis[(vectors,)])
 
             for k, b in zip(vectors, s_basis):
                 x, y = b[idxs[plane]]
                 l = r" ${}_{} $".format(_label, k + 1)
                 l = l + "\n" if y < 0 else "\n" + l
                 ha = "right" if x < 0 else "left"
@@ -991,26 +1015,21 @@
             if zoffset > zmax:
                 zmax = zoffset
             elif zoffset < zmin:
                 zmin = zoffset
             ax.set_zlim([zmin, zmax])
         else:
             ax.set_aspect("equal")  # Must for 2D axes to show actual lengths of BZ
-        return ax
+
     else:  # Plot 3D
-        if getattr(ax, "name", "") == "3d":  # handle None or 2D axes passed.
-            ax3d = ax
-        else:
-            pos = ax.get_position()
-            fig = ax.get_figure()
-            ax.remove()
-            ax3d = fig.add_axes(
-                pos, projection="3d", azim=45, elev=30, proj_type="ortho"
-            )
-            type(bz_data)._splot_kws["ax"] = ax3d
+        if not ax:  # For 3D.
+            ax = ptk.get_axes(figsize=(3.4, 3.4), axes_3d=True)
+
+        if getattr(ax, "name", "") != "3d":
+            raise ValueError("3D axes required for 3D plot.")
 
         if fill:
             if colormap:
                 colormap = colormap if colormap in plt.colormaps() else "viridis"
                 cz = [
                     np.mean(np.unique(f, axis=0), axis=0)[2]
                     for f in bz_data.faces_coords
@@ -1028,70 +1047,161 @@
                 facecolors=colors,
                 alpha=alpha,
                 shade=shade,
                 label=name,
                 **kwargs,
             )
 
-            ax3d.add_collection(poly)
-            ax3d.autoscale_view()
+            ax.add_collection(poly)
+            ax.autoscale_view()
         else:
             kwargs = {"solid_capstyle": "round", **kwargs}
             (line,) = [
-                ax3d.plot3D(f[:, 0], f[:, 1], f[:, 2], color=(color), **kwargs)
+                ax.plot3D(f[:, 0], f[:, 1], f[:, 2], color=(color), **kwargs)
                 for f in bz_data.faces_coords
             ][0]
             line.set_label(name)  # only one line
 
-        if vectors:
+        if vectors and not is_subzone:
             for k, v in enumerate(0.35 * bz_data.basis):
-                ax3d.text(
-                    *v, r"${}_{}$".format(_label, k + 1), va="center", ha="center"
-                )
+                ax.text(*v, r"${}_{}$".format(_label, k + 1), va="center", ha="center")
 
             XYZ, UVW = [[0, 0, 0], [0, 0, 0], [0, 0, 0]], 0.3 * bz_data.basis.T
             quiver3d(
-                *XYZ, *UVW, C="k", L=0.7, ax=ax3d, arrowstyle="-|>", mutation_scale=7
+                *XYZ, *UVW, C="k", L=0.7, ax=ax, arrowstyle="-|>", mutation_scale=7
             )
 
         l_ = np.min(bz_data.vertices, axis=0)
         h_ = np.max(bz_data.vertices, axis=0)
-        ax3d.set_xlim([l_[0], h_[0]])
-        ax3d.set_ylim([l_[1], h_[1]])
-        ax3d.set_zlim([l_[2], h_[2]])
+        ax.set_xlim([l_[0], h_[0]])
+        ax.set_ylim([l_[1], h_[1]])
+        ax.set_zlim([l_[2], h_[2]])
 
         # Set aspect to same as data.
-        ax3d.set_box_aspect(np.ptp(bz_data.vertices, axis=0))
+        ax.set_box_aspect(np.ptp(bz_data.vertices, axis=0))
+
+        ax.set_xlabel(label.format("x"))
+        ax.set_ylabel(label.format("y"))
+        ax.set_zlabel(label.format("z"))
+
+    if vname == "b":  # These needed for splot_kpath internally
+        type(bz_data)._splot_kws = dict(plane=plane, zoffset=zoffset, ax=ax)
+
+    return ax
+
+
+def splot_kpath(
+    bz_data, kpoints, labels=None, fmt_label=lambda x: (x, {"color": "blue"}), **kwargs
+):
+    """Plot k-path over existing BZ. It will take ``ax``, ``plane`` and ``zoffset`` internally from most recent call to ``splot_bz``/``bz.splot``.
+
+    Parameters
+    ----------
+    kpoints : array_like
+        List of k-points in fractional coordinates. e.g. [(0,0,0),(0.5,0.5,0.5),(1,1,1)] in order of path.
+    labels : list
+        List of labels for each k-point in same order as kpoints.
+    fmt_label : callable
+        Function that takes a label from labels and should return a string or (str, dict) of which dict is passed to ``plt.text``.
+
+
+    kwargs are passed to ``plt.plot`` with some defaults.
+
+    You can get ``kpoints = POSCAR.get_bz().specials.masked(lambda x,y,z : (-0.1 < z 0.1) & (x >= 0) & (y >= 0))`` to get k-points in positive xy plane.
+    Then you can reorder them by an indexer like ``kpoints = kpoints[[0,1,2,0,7,6]]``, note double brackets, and also that point at zero index is taken twice.
+
+    .. tip::
+        You can use this function multiple times to plot multiple/broken paths over same BZ.
+    """
+    if not hasattr(bz_data, "_splot_kws"):
+        raise ValueError("Plot BZ first to get ax, plane and zoffset.")
+
+    if not np.ndim(kpoints) == 2 and np.shape(kpoints)[-1] == 3:
+        raise ValueError("kpoints must be 2D array of shape (N,3)")
+
+    plane, ax, zoffset = [
+        bz_data._splot_kws.get(attr, default)  # class level attributes
+        for attr, default in zip(["plane", "ax", "zoffset"], [None, None, 0])
+    ]
+
+    ijk = [0, 1, 2]
+    _mapping = {
+        "xy": [0, 1],
+        "xz": [0, 2],
+        "yz": [1, 2],
+        "zx": [2, 0],
+        "zy": [2, 1],
+        "yx": [1, 0],
+    }
+    _zoffset = [0, 0, 0]
+    if plane:
+        _zoffset = (
+            [0, 0, zoffset]
+            if plane in "xyx"
+            else [0, zoffset, 0]
+            if plane in "xzx"
+            else [zoffset, 0, 0]
+        )
 
-        ax3d.set_xlabel(label.format("x"))
-        ax3d.set_ylabel(label.format("y"))
-        ax3d.set_zlabel(label.format("z"))
-        return ax3d
+    if isinstance(plane, str) and plane in _mapping:
+        if getattr(ax, "name", None) != "3d":
+            ijk = _mapping[
+                plane
+            ]  # only change indices if axes is not 3d, even if plane is given
+
+    if not labels:
+        labels = [
+            "[{0:5.2f}, {1:5.2f}, {2:5.2f}]".format(x, y, z) for x, y, z in kpoints
+        ]
+
+    _validate_label_func(fmt_label, labels[0])
+
+    coords = bz_data.to_cartesian(kpoints)
+    if _zoffset and plane:
+        normal = (
+            [0, 0, 1] if plane in "xyx" else [0, 1, 0] if plane in "xzx" else [1, 0, 0]
+        )
+        coords = to_plane(normal, coords) + _zoffset
+
+    coords = coords[:, ijk]  # select only required indices
+    kwargs = {
+        **dict(color="blue", linewidth=0.8, marker=".", markersize=10),
+        **kwargs,
+    }  # need some defaults
+    ax.plot(*coords.T, **kwargs)
+
+    for c, text in zip(coords, labels):
+        lab, textkws = fmt_label(text), {}
+        if isinstance(lab, (list, tuple)):
+            lab, textkws = lab
+        ax.text(*c, lab, **textkws)
+
+    return ax
 
 
 # Cell
 def iplot_bz(
     bz_data,
     fill=False,
-    color="rgba(168,204,216,0.8)",
+    color="rgba(84,102,108,0.8)",
     special_kpoints=True,
     alpha=0.4,
     ortho3d=True,
     fig=None,
     **kwargs,
 ):
     """Plots interactive figure showing axes,BZ surface, special points and basis, each of which could be hidden or shown.
 
     Parameters
     ----------
     bz_data : Output of `get_bz`.
     fill : bool
         False by defult, determines whether to fill surface of BZ or not.
     color : str
-        Color to fill surface 'rgba(168,204,216,0.4)` by default. This sholud be a valid Plotly color.
+        Color to fill surface 'rgba(84,102,108,0.8)` by default. This sholud be a valid Plotly color.
     special_kpoints : bool or callable
         True by default, determines whether to plot special points or not.
         You can also proivide a mask function f(x,y,z) -> bool which will be used to filter special points
         based on their fractional coordinates. This is ignored if BZ is primitive.
     alpha : float
         Opacity of BZ planes.
     ortho3d : bool
@@ -1117,100 +1227,108 @@
         "",
         "<b>k</b><sub>z</sub>/2π",
     ]
     if vname == "a":
         axes_text = ["<b>x</b>", "", "<b>y</b>", "", "<b>z</b>"]  # Real space
 
     zone_name = kwargs.pop("name", "BZ" if vname == "b" else "Lattice")
-    # Axes
-    _len = 0.5 * np.mean(bz_data.basis)
-    fig.add_trace(
-        go.Scatter3d(
-            x=[_len, 0, 0, 0, 0],
-            y=[0, 0, _len, 0, 0],
-            z=[0, 0, 0, 0, _len],
-            mode="lines+text",
-            text=axes_text,
-            line_color="skyblue",
-            legendgroup="Axes",
-            name="Axes",
-        )
-    )
-    fig.add_trace(
-        go.Cone(
-            x=[_len, 0, 0],
-            y=[0, _len, 0],
-            z=[0, 0, _len],
-            u=[1, 0, 0],
-            v=[0, 1, 0],
-            w=[0, 0, 1],
-            showscale=False,
-            sizemode="absolute",
-            sizeref=0.5,
-            anchor="tail",
-            colorscale=["skyblue" for _ in range(3)],
-            legendgroup="Axes",
-            name="Axes",
-        )
-    )
+    is_subzone = hasattr(bz_data, "_specials")  # For subzone
 
-    # Basis
-    for i, b in enumerate(bz_data.basis):
+    if not is_subzone:  # No basis, axes for subzone
+        # Axes
+        _len = 0.5 * np.mean(bz_data.basis)
         fig.add_trace(
             go.Scatter3d(
-                x=[0, b[0]],
-                y=[0, b[1]],
-                z=[0, b[2]],
+                x=[_len, 0, 0, 0, 0],
+                y=[0, 0, _len, 0, 0],
+                z=[0, 0, 0, 0, _len],
                 mode="lines+text",
-                legendgroup="{}<sub>{}</sub>".format(vname, i + 1),
-                line_color="red",
-                name="<b>{}</b><sub>{}</sub>".format(vname, i + 1),
-                text=["", "<b>{}</b><sub>{}</sub>".format(vname, i + 1)],
+                text=axes_text,
+                line_color="skyblue",
+                legendgroup="Axes",
+                name="Axes",
             )
         )
-
-        uvw = b / np.linalg.norm(b)  # Unit vector for cones
         fig.add_trace(
             go.Cone(
-                x=[b[0]],
-                y=[b[1]],
-                z=[b[2]],
-                u=uvw[0:1],
-                v=uvw[1:2],
-                w=uvw[2:],
+                x=[_len, 0, 0],
+                y=[0, _len, 0],
+                z=[0, 0, _len],
+                u=[1, 0, 0],
+                v=[0, 1, 0],
+                w=[0, 0, 1],
                 showscale=False,
-                colorscale="Reds",
                 sizemode="absolute",
-                sizeref=0.02,
+                sizeref=0.5,
                 anchor="tail",
-                legendgroup="{}<sub>{}</sub>".format(vname, i + 1),
-                name="<b>{}</b><sub>{}</sub>".format(vname, i + 1),
+                colorscale=["skyblue" for _ in range(3)],
+                legendgroup="Axes",
+                name="Axes",
             )
         )
 
+        # Basis
+        for i, b in enumerate(bz_data.basis):
+            fig.add_trace(
+                go.Scatter3d(
+                    x=[0, b[0]],
+                    y=[0, b[1]],
+                    z=[0, b[2]],
+                    mode="lines+text",
+                    legendgroup="{}<sub>{}</sub>".format(vname, i + 1),
+                    line_color="red",
+                    name="<b>{}</b><sub>{}</sub>".format(vname, i + 1),
+                    text=["", "<b>{}</b><sub>{}</sub>".format(vname, i + 1)],
+                )
+            )
+
+            uvw = b / np.linalg.norm(b)  # Unit vector for cones
+            fig.add_trace(
+                go.Cone(
+                    x=[b[0]],
+                    y=[b[1]],
+                    z=[b[2]],
+                    u=uvw[0:1],
+                    v=uvw[1:2],
+                    w=uvw[2:],
+                    showscale=False,
+                    colorscale="Reds",
+                    sizemode="absolute",
+                    sizeref=0.02,
+                    anchor="tail",
+                    legendgroup="{}<sub>{}</sub>".format(vname, i + 1),
+                    name="<b>{}</b><sub>{}</sub>".format(vname, i + 1),
+                )
+            )
+
+    # Rest of the code is same for both subzone and BZ/Cell
     # Faces
     legend = True
     for pts in bz_data.faces_coords:
         fig.add_trace(
             go.Scatter3d(
                 x=pts[:, 0],
                 y=pts[:, 1],
                 z=pts[:, 2],
                 mode="lines",
                 line_color=color,
                 legendgroup=zone_name,
                 name=zone_name,
                 showlegend=legend,
+                surfaceaxis=2 if fill and coplanar(bz_data.vertices) else -1,
+                surfacecolor=color,  # fills z-axis because its where 2D projection is
+                opacity=alpha,
                 **kwargs,
             )
         )
 
         legend = False  # Only first legend to show for all
 
-    if fill:
+    if fill and not coplanar(bz_data.vertices):
+        # coplanar fill is not supported by Mesh3d
         xc = bz_data.vertices[ConvexHull(bz_data.vertices).vertices]
         fig.add_trace(
             go.Mesh3d(
                 x=xc[:, 0],
                 y=xc[:, 1],
                 z=xc[:, 2],
                 color=color,
```

### Comparing `ipyvasp-0.4.0/ipyvasp/bsdos.py` & `ipyvasp-0.5.0/ipyvasp/bsdos.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.4.0/ipyvasp/core/parser.py` & `ipyvasp-0.5.0/ipyvasp/core/parser.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.4.0/ipyvasp/core/plot_toolkit.py` & `ipyvasp-0.5.0/ipyvasp/core/plot_toolkit.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.4.0/ipyvasp/core/serializer.py` & `ipyvasp-0.5.0/ipyvasp/core/serializer.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,25 @@
 import inspect
 from collections import namedtuple
 from copy import deepcopy
 from pathlib import Path
 
 import numpy as np
 
-from .spatial_toolkit import angle_deg, to_basis, to_R3, kpoints2bz, get_bz
+from .spatial_toolkit import (
+    angle_deg,
+    to_basis,
+    to_R3,
+    kpoints2bz,
+    order,
+    coplanar,
+    angle_deg,
+    ConvexHull,
+)
+from ..utils import _sub_doc
 
 
 def dict2tuple(name: str, d: dict):
     """
     Converts a dictionary (nested as well) to namedtuple, accessible via index and dot notation as well as by unpacking.
 
     Parameters
@@ -415,29 +425,14 @@
 
         mask = [func(x, y, z) for x, y, z in self.kpoints]
         return SpecialPoints(
             {"coords": self.coords[mask], "kpoints": self.kpoints[mask]}
         )
 
 
-class SubZoneData(Dict2Data):
-    _req_keys = ("vertices", "faces", "specials")
-
-    def __init__(self, d):
-        super().__init__(d)
-
-    def splot(plane=None):
-        # Implemenet using splot under BrZoneData
-        raise NotImplementedError("Not implemented yet")
-
-    def iplot():
-        # Implemenet using iplot under BrZoneData
-        raise NotImplementedError("Not implemented yet")
-
-
 def _methods_imported():
     # These imports work as methods of the class
     from .._lattice import splot_bz as splot, iplot_bz as iplot  # Avoid circular import
 
     splot.__doc__ = re.sub(  # This replaces orginal docstring too. That is strange
         "bz_data :.*plane :", "plane :", splot.__doc__, flags=re.DOTALL
     )
@@ -445,36 +440,41 @@
         "bz_data :.*fill :", "fill :", iplot.__doc__, flags=re.DOTALL
     )
     return splot, iplot
 
 
 class BrZoneData(Dict2Data):
     splot, iplot = _methods_imported()
+    from .._lattice import splot_kpath  # no change in this
+
     _req_keys = ("basis", "faces", "vertices", "primitive")
 
     def __init__(self, d):
         super().__init__(d)
 
     def get_special_points(self, orderby=(1, 1, 1)):
         """Returns the special points in the brillouin zone in the order relative
         to a given point in cartesian coordinates. Gamma is always first."""
         if self.primitive:
             return SpecialPoints(
                 {"coords": np.empty((0, 3)), "kpoints": np.empty((0, 3))}
             )  # Primitive Zone has no meaning for special points
 
+        if hasattr(self, "_specials"):  # Transformed BZ
+            return self._specials
+
         mid_faces = np.array(
             [np.mean(np.unique(face, axis=0), axis=0) for face in self.faces_coords]
         )
         mid_edges = []
-        for f in self.faces_coords:
-            for i in range(len(f) - 1):
+        for face in self.faces_coords:
+            for f, g in zip(face[:-1], face[1:]):
                 # NOTE: Do not insert point between unique vertices, is it necessary?
-                if np.isclose(np.linalg.norm(f[i]), np.linalg.norm(f[i + 1])):
-                    mid_edges.append(np.mean([f[i], f[i + 1]], axis=0))
+                if np.isclose(np.linalg.norm(f), np.linalg.norm(g)):
+                    mid_edges.append(np.mean([f, g], axis=0))
 
         if mid_edges != []:
             mid_edges = np.unique(mid_edges, axis=0)  # because faces share edges
             mid_faces = np.concatenate([mid_faces, mid_edges])
 
         # Bring all high symmetry points together.
         sp_carts = np.concatenate(
@@ -543,31 +543,72 @@
         """
         if not isinstance(other, self.__class__):
             raise TypeError(
                 f"other must be a {self.__class__} object, got {type(other)}"
             )
         return other.to_fractional(self.to_cartesian(kpoints))
 
-    def translate_inside(self, kpoints, shift=0):
-        """Brings kpoints inside BZ. Mostly useful for regular kmesh to bring all kpoints inside BZ.
-        `shift` is a number or a list of three numbers that will be added to kpoints before any other operation,
-        in case points are not symmetric around origin.
+    @_sub_doc(kpoints2bz, {"bz_data :.*kpoints :": "kpoints :"})
+    def translate_inside(self, kpoints, shift=0, keep_geometry=False):
+        return kpoints2bz(self, kpoints, shift=shift, keep_geomerty=keep_geometry)
+
+    def subzone(self, func, loop=True):
+        """Returns a subzone of the brillouin zone by applying a function on the fractional special points of the zone.
+
+        .. tip::
+            You can get a 2D subzone by using ``lambda x,y,z: -0.1 < z < 0.1`` where 0.1 is taken as a tolerance.
 
         .. warning::
-            If you made cartesian kpoints, you should not translate them with this function, just shift them by adding a vector.
+            We do not check if output is an irreducible zone or not. It is just a subzone based on the function.
         """
-        return kpoints2bz(self, kpoints, shift=shift)
+        try:
+            out = func(0, 0, 0)
+            if not isinstance(out, bool):
+                raise TypeError(f"func must return bool, got {type(out)}")
+        except:
+            raise TypeError(f"func must be callable with 3 arguments, got {type(func)}")
+
+        spoints = self.specials.kpoints
+        fverts = []
+        for vert in spoints:
+            if func(*vert):
+                fverts.append(vert)
+
+        if len(fverts) < 3:
+            raise ValueError(
+                "subzone should at least have 3 special points. Try another function."
+            )
+
+        cverts = self.to_cartesian(fverts)
+        specials = SpecialPoints(
+            {"kpoints": np.array(fverts), "coords": cverts}
+        )  # save befor other operations
+
+        if coplanar(cverts):
+            verts = cverts[order(cverts, loop=False)]
+            if tuple(verts[0]) == (0, 0, 0):  # gamma is first always
+                if angle_deg(verts[1], verts[-1]) < 90:
+                    verts = verts[1:]  # remove gamma to avoid concavity
+
+            vertices = np.vstack([verts, verts[:1]]) if loop else verts
+            faces = [list(range(len(vertices)))]  # still list of list
+        else:
+            chull = ConvexHull(cverts)
+            vertices = cverts[chull.vertices]  # those are indices
 
-    def get_subzone(self, func):
-        # Disclaimer: Reuduction totally depends on given function, we only test for volume to satify the condition V_old = N * V_new
-        # This should add an attrivute to not recalculate special points, just return old points including in this zone
-        # How to plot the reduced zone, as it will be nowhere? or make this a plotting function? or add new namespace to POSACR? like splot_bzr(func), thing?
-        # return SubZoneData({"vertices","faces", "specials"})
-        # specials here should not be recalculated, old ones with in this zone
-        raise NotImplementedError("Not implemented yet")
+            vertidx = chull.vertices.tolist()
+            faces = []
+            for sim in chull.simplices.tolist():
+                face = [vertidx.index(s) for s in sim]
+                faces.append(face)
+            # TODO: Merge faces if they share an edge and are coplanar using simplify_faces from spatial_toolkit
+
+        d = self.copy().to_dict()
+        d.update({"faces": faces, "vertices": vertices, "_specials": specials})
+        return self.__class__(d)
 
 
 class CellData(Dict2Data):
     splot, iplot = _methods_imported()
     _req_keys = ("basis", "faces", "vertices")
 
     def __init__(self, d):
```

### Comparing `ipyvasp-0.4.0/ipyvasp/core/spatial_toolkit.py` & `ipyvasp-0.5.0/ipyvasp/core/spatial_toolkit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from itertools import product
+from itertools import product, combinations
+from collections import Iterable
 
 import numpy as np
 from scipy.spatial.transform import Rotation
 from scipy.spatial import ConvexHull, Voronoi
 
 
 def tan_inv(vy, vx):
@@ -61,15 +62,20 @@
     # Fix points if start point is zero.
     if np.sum(points[0]) == 0:
         points = points + 0.5
 
     center = np.mean(points, axis=0)  # 3D cent point.
     vectors = points - center  # Relative to center
 
-    ex = vectors[0] / np.linalg.norm(vectors[0])  # i
+    for v in vectors:
+        start = v  # Start with first non-zero vector.
+        if not np.allclose(start, [0, 0, 0]):
+            break
+
+    ex = start / np.linalg.norm(start)  # i
     ey = np.cross(center, ex)
     ey = ey / np.linalg.norm(ey)  # j
 
     angles = []
     for i, v in enumerate(vectors):
         vx = np.dot(v, ex)
         vy = np.dot(v, ey)
@@ -140,14 +146,31 @@
     [-0.3660254  1.3660254  1.]
     """
     axis_vec = np.array(axis_vec) / np.linalg.norm(axis_vec)  # Normalization
     angle_rad = np.deg2rad(angle_deg)
     return Rotation.from_rotvec(angle_rad * axis_vec)
 
 
+def coplanar(points, tol=1e-5):
+    """Returns true if points are coplanar within `tol` tolerance."""
+    if np.ndim(points) != 2 and np.shape(points)[-1] != 3:
+        raise ValueError("points should be a 2D array of shape (N,3).")
+    if len(points) < 3:
+        raise ValueError("points should have at least 3 points.")
+
+    points = np.array(points)
+    have_volume = []
+    for p1, p2, p3 in combinations(points, 3):
+        if np.abs(p1.dot(np.cross(p2, p3))) < np.abs(tol):
+            have_volume.append(False)
+        else:
+            have_volume.append(True)
+    return not any(have_volume)  # If all are coplanar.
+
+
 def inside_convexhull(hull, points):
     if not isinstance(hull, ConvexHull):
         raise TypeError("hull must be a scipy.spatial.ConvexHull object")
 
     if np.shape(points)[-1] != hull.points.shape[-1]:
         raise ValueError("points must have same physical dimension as hull.points")
 
@@ -294,28 +317,30 @@
         "primitive": primitive,
     }
     from .serializer import BrZoneData  # to avoid circular import
 
     return BrZoneData(out_dict)
 
 
-def kpoints2bz(bz_data, kpoints, shift=0):
-    """Brings KPOINTS inside BZ. Applies `to_R3` only if bz_data is for primitive BZ.
+def kpoints2bz(bz_data, kpoints, shift=0, keep_geomerty=False):
+    """Brings KPOINTS inside BZ. Applies `to_R3` only if BZ is primitive.
 
     Parameters
     ----------
     bz_data : Output of get_bz().
-    kpoints : List or array of KPOINTS to transorm into BZ or R3.
-    shift : This value is added to kpoints before any other operation, single number of list of 3 numbers for each direction.
-
-    .. warning::
-        Do not use this function to translate kpoints created as cartesian, just shift by adding a vector.
+    kpoints : array_like
+        List or array of KPOINTS to transorm into BZ or R3.
+    shift : float
+        This value is added to kpoints before any other operation, single number of list of 3 numbers for each direction.
+    keep_geomerty : bool
+        If True, returns kpoints in R3 with `shift` applied, keeping the neighbors in order, else kpoints adopt the shape of BZ.
+        This is useful when you already created cartesian kpoints mesh and want to collect their fractional coordinates back to cartesian.
     """
     kpoints = np.array(kpoints) + shift
-    if bz_data.primitive:
+    if bz_data.primitive or keep_geomerty:
         return to_R3(bz_data.basis, kpoints)
 
     cent_planes = [
         np.mean(np.unique(face, axis=0), axis=0) for face in bz_data.faces_coords
     ]
 
     out_coords = np.empty(np.shape(kpoints))  # To store back
@@ -338,7 +363,58 @@
             r = inside(pos, cent_planes)
             if r:
                 # print(p,'-->',r)
                 out_coords[i] = r
                 StopIteration
 
     return out_coords  # These may have duplicates, apply np.unique(out_coords,axis=0). do this in surface plots
+
+
+def simplify_faces(vertices, faces, loop=True):
+    """Simplifies faces by merging adjacent coplanar faces.
+
+    Parameters
+    ----------
+    vertices : array_like
+        List of vertices of faces. Should be cartesian coordinates.
+    faces : array_like
+        List of faces, each face is a list of indices of vertices.
+    loop : bool
+        If True, joins the last vertex of a face to starting vertex in order to complete loop.
+
+    Returns
+    -------
+    faces
+    """
+    if np.ndim(vertices) != 2 and np.shape(vertices)[1] != 3:
+        raise ValueError("vertices must be a Nx3 array.")
+    if not isinstance(faces, Iterable):
+        raise ValueError("faces must be an iterable.")
+    for face in faces:
+        if not isinstance(face, Iterable):
+            raise ValueError("faces must be an iterable of iterables.")
+        for idx in face:
+            if not isinstance(idx, (int, np.integer)):
+                raise ValueError("faces must be an iterable of iterables of integers.")
+    raise NotImplementedError("This function is not ready yet.")
+
+    # TODO: This needs a lot of thoughts
+    # new_faces = []
+    # for fi in faces:
+    #     face = list(fi)
+    #     for fj in faces:
+    #         if fi != fj:
+    #             if len(set(face) & set(fj)) >= 2 and coplanar(vertices[[*face, *fj]]):
+    #                 face.extend(fj)  # adjacent and coplanar face
+    #     # else:
+    #     #     new_faces.append(fi)
+    #     new_faces.append(list(set(face)))  # remove duplicates
+
+    new_faces = list(reversed(sorted(new_faces, key=len)))  # sort by number of vertices
+    # Remove overlapping faces
+    unique_faces = new_faces[:1]  # first face is always unique
+    for face in new_faces[1:]:
+        if not any(set(face).issubset(f) for f in unique_faces):
+            _order = order(vertices[face], loop=loop)
+            unique_faces.append([face[i] for i in _order])
+
+    return unique_faces
```

### Comparing `ipyvasp-0.4.0/ipyvasp/evals_dataframe.py` & `ipyvasp-0.5.0/ipyvasp/evals_dataframe.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.4.0/ipyvasp/misc.py` & `ipyvasp-0.5.0/ipyvasp/misc.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.4.0/ipyvasp/potential.py` & `ipyvasp-0.5.0/ipyvasp/potential.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.4.0/ipyvasp/utils.py` & `ipyvasp-0.5.0/ipyvasp/utils.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.4.0/ipyvasp/widgets.py` & `ipyvasp-0.5.0/ipyvasp/widgets.py`

 * *Files identical despite different names*

### Comparing `ipyvasp-0.4.0/ipyvasp.egg-info/PKG-INFO` & `ipyvasp-0.5.0/ipyvasp.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyvasp
-Version: 0.4.0
+Version: 0.5.0
 Summary: A processing tool for VASP DFT input/output processing in Jupyter Notebook.
 Home-page: https://github.com/massgh/ipyvasp
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyvasp/issues
 Keywords: Jupyter,Widgets,IPython,VASP,DFT
```

### Comparing `ipyvasp-0.4.0/ipyvasp.egg-info/SOURCES.txt` & `ipyvasp-0.5.0/ipyvasp.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 ipyvasp/misc.py
 ipyvasp/potential.py
 ipyvasp/utils.py
 ipyvasp/widgets.py
 ipyvasp.egg-info/PKG-INFO
 ipyvasp.egg-info/SOURCES.txt
 ipyvasp.egg-info/dependency_links.txt
+ipyvasp.egg-info/entry_points.txt
 ipyvasp.egg-info/requires.txt
 ipyvasp.egg-info/top_level.txt
 ipyvasp/core/__init__.py
 ipyvasp/core/parser.py
 ipyvasp/core/plot_toolkit.py
 ipyvasp/core/serializer.py
 ipyvasp/core/spatial_toolkit.py
```

### Comparing `ipyvasp-0.4.0/setup.py` & `ipyvasp-0.5.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,8 +121,14 @@
     ],
     keywords=KEYWORDS,
     project_urls=PROJECT_URLS,
     # $ setup.py publish support.
     cmdclass={
         "upload": UploadCommand,
     },
+    # for command line interface
+    entry_points={
+        "console_scripts": [
+            "ipyvasp=ipyvasp.cli:main",
+        ]
+    },
 )
```

