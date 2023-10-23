# Ink-Detection-Resurrect-an-ancient-library-from-the-ashes-of-a-volcano

Introduction

This repository contains the resources focused on detecting ink in 3D X-ray scans of ancient papyrus fragments. This challenge is a subproblem of solving the Vesuvius Challenge, with the ultimate goal of recovering and preserving ancient scrolls discovered in Herculaneum, which were buried by the eruption of Mount Vesuvius almost 2,000 years ago.

Problem Statement

The challenge revolves around identifying the presence of ink in 3D X-ray scans of detached fragments of ancient papyrus scrolls. The ink used in the Herculaneum scrolls is not easily visible in X-ray scans, but machine learning models have shown promise in detecting it. Fortunately, there's ground truth data available for training and validation.

Dataset

The dataset provided includes:

3D X-ray scans of four fragments at 4µm resolution, obtained using a particle accelerator.

Infrared photographs of the surface of the fragments that show visible ink, which have been aligned with the X-ray scans.

Hand-labeled binary masks indicating the presence of ink in the photographs.

File Structure

train/test/[fragment_id]/surface_volume/[image_id].tif: Greyscale slices from the 3D X-ray surface volume.

train/test/[fragment_id]/mask.png: Binary masks indicating which pixels contain data.

train/[fragment_id]/inklabels.png: Binary masks for ink vs. no-ink labels.

train/[fragment_id]/inklabels_rle.csv: Run-length-encoded version of the labels, generated using a provided script.

train/[fragment_id]/ir.png: Infrared photos that form the basis of the binary mask.

