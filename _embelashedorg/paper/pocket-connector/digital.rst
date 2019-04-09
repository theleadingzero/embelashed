Digital Pocket Connector
########################

.. image:: ./imgs/digital-pocket-banner.jpg
  :alt: Photo of Digital Pocket Connecter.

The Digital Pocket Connector connects digital sensor circuits to the Paper Capelet. It breaks out the 3.3V, GND, and digital GPIO pin connections on the Grove connector. These are electrically connected to a folded paper pocket that then provides a mechanical and electrical connection to the sensing circuit.

You need to order or fabricate the printed circuit board (PCB), and then can add the rest of the components.

.. image:: https://oshpark.com/assets/badge-5b7ec47045b78aef6eb9d83b3bac6b1920de805e9a0c227658eac6e19a045b9c.png
  :alt: "Order from OSH Park"
  :target: https://oshpark.com/shared_projects/Fme4UGC4


Building the Digital Pocket Connector
*************************************


You will need
=============

* Digital Pocket Connector PCB
* Grove horizontal DIP connector 
* Paper template
* Strip of 0.25"/5mm copper tape  
* Scotch/Sello tape 
* Soldering equipment


Steps
=====
1. Order directly or download the gbr files from `OSH Park <https://oshpark.com/shared_projects/Fme4UGC4>`_ and fabricate the PCB.
  
  .. image:: ./imgs/digital-pcb.jpg
    :width: 400
    :alt: Photo of PCB from OSH Park.

2. Solder the Grove connector to the PCB, following the outline of the silkscreen.
  
  .. image:: ./imgs/pocket-digital-soldered.jpg
    :width: 400
    :alt: Photo of PCB with Grove connector soldered.

3. Download the template from the `embelashed repository <https://github.com/theleadingzero/embelashed/tree/master/paper/pocket-connector-cutting-files/analog-digital>`_. The `.studio3` file is for a `Silhouette machine <https://www.silhouetteamerica.com/>`_ and the other files can be used with a printer or laser cutter. The red lines are where the template should be cut and the blue lines are where an outline should be drawn. 

4. Cut out the paper template using your preferred method.    
  
  .. image:: ./imgs/template-3.jpg
    :width: 400
    :alt: Photo of paper template cutout and with guide outlines drawn.

5. Cut the copper tape in half lengthwise with a pair of scissors.

  .. image:: ./imgs/cut_24_0-18.gif
    :alt: Animation of cutting copper tape.

6. Stick the three pieces of copper tape onto the paper template, following the outlines.
  
  .. image:: ./imgs/copper-paper-3.jpg
    :width: 400
    :alt: Photo of paper template with copper tape.

7. Fold the template along the guidelines. Start by folding the template in half with the copper tape on the inside. Then fold along the other two lines to create an accordion shape.
   
  .. image:: ./imgs/accordion-3.jpg  
    :width: 400 
    :alt: Photo of folded template in accordion shape.

8. Identify the side of the folded template with an outline that matches the edge of the PCB. It is also the side with more copper tape. Place that side on the top of the PCB, lining up the outline with the edge of the PCB.

9. Using non-conductive tape like scotch/sello tape, tape the paper template to the PCB, taking care to leave open the pocket edge. 
  
  .. image:: ./imgs/pocket-digital-complete.jpg
    :height: 300
    :alt: Photo of top of completed Pocket Connector.

  .. image:: ./imgs/pocket-underside.jpg
    :height: 300
    :alt: Photo of bottom of completed Pocket Connector.

.. warning::
  `embelashed` uses Grove connectors to connect Pocket Connectors to the Paper Capelet, but be aware that the Analog and Digital Pocket Connectors do not follow the standard pin arrangement found in other Grove sensors.

