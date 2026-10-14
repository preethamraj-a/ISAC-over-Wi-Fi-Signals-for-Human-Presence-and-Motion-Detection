# ISAC over Wi-Fi Signals for Human Presence and Motion Detection

GNU Radio-based OFDM system for Wi-Fi-band integrated sensing and communication, with Doppler and multipath analysis.

## Overview

This project demonstrates a laboratory-scale Integrated Sensing and Communication (ISAC) system based on an OFDM wireless communication system. Developed as a team project for my bachelor's thesis at the Keysight RFCoE 5G Lab, SASTRA Deemed University, India, the system was designed to investigate Doppler-related changes and multipath propagation associated with human presence and motion while maintaining data transmission between the transmitter and receiver.

## System Design

GNU Radio Companion was used to design the OFDM transmitter and receiver flowgraphs. The simulation workflow incorporated Doppler injection and a multi-ray propagation model. The receiver processing involved synchronisation, channel estimation, and equalisation.

Although an existing OFDM transmitter block provided built-in synchronisation, equalisation, and other processing functions, we aimed to ensure consistency in sample rates and FFT sizes throughout the system. We also considered the possibility of adjusting individual block parameters during subsequent development.

## Hardware and Experimental Setup

The experimental setup used an NI USRP-2910 software-defined radio (SDR). Other tools included Keysight SystemVue for studying multipath propagation using an actual Wi-Fi 5 OFDM signal, GNU Radio for designing the flowgraphs, RF signal analysers and generators, and horn and whip antennas for measurements.

An anechoic chamber was also used during the initial phase of the project to investigate Doppler-related effects and multipath propagation under controlled conditions.

## Key Technical Work

- Used a peak detector to extract Doppler-related frequency variations from oscillations in the channel response. We also observed delay bins associated with multipath propagation and compared measurements in an environment with human presence against measurements obtained in an anechoic chamber during the initial phase of the project.
- Investigated Doppler extraction by analysing phase variations in the BPSK-modulated pilot subcarriers of the OFDM signal.

## Repository Contents

This repository documents the system architecture, experimental approach, and selected project figures. The original laboratory GNU Radio flowgraph files are not included because access to them is restricted by laboratory rules.

Only materials authorised for public sharing will be uploaded.

## Project Context

Bachelor's thesis in Electronics and Communication Engineering, SASTRA Deemed University, India.
