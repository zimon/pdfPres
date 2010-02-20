# -*- coding: utf-8 -*-


# Set up environment, pkg-config for GTK/poppler, ...
env = Environment(CCFLAGS = '-Wall -Wextra')
env.SetOption('num_jobs', 4)
env.ParseConfig('pkg-config --cflags --libs gtk+-2.0 poppler-glib')
env.ParseConfig('xml2-config --cflags --libs')

# Build instructions
env.Program('pdfPres', Glob('*.c'))
